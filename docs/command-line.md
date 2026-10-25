# Command line

Every button in the windows runs `hypersuite.exe` itself with one of the
commands below, so everything the apps do can also be scripted.

```
hypersuite                      open the launcher
hypersuite gui --app <app>      open one app: scan, sort or mail
hypersuite index <args...>      Scan: indexing and reports        (hypersuite index --help)
hypersuite file <args...>       Sort: the library                 (hypersuite file --help)
hypersuite mail <args...>       Outbird: Outlook to Thunderbird   (hypersuite mail --help)
hypersuite tools [--verify|--reset]
hypersuite --version
```

`hypersuite <command> --help` and `hypersuite <command> <subcommand> --help`
print the full help, with examples. The built-in help still uses the names of
the three engines (`hyperindex`, `hyperfiler`, `outbird`); read them as
`hypersuite index`, `hypersuite file` and `hypersuite mail`.

**cmd doesn't wait for hypersuite.** The exe is a windowed program, so cmd
returns immediately and the output appears after the prompt. Use:

```bat
start /wait hypersuite index stats
```

In PowerShell, pipe it: `hypersuite index stats | Out-Host`. In batch files,
`start /wait` also makes `%ERRORLEVEL%` meaningful (0 = success).

Contents:
[index](#hypersuite-index--scan-and-reports) ·
[file](#hypersuite-file--sort) ·
[mail](#hypersuite-mail--outlook-to-thunderbird) ·
[tools](#hypersuite-tools) ·
[environment variables](#environment-variables)

---

## hypersuite index — Scan and reports

Options for every `index` command:

| Option | Meaning |
|---|---|
| `--db <path>` | The index database. Default for the command line: `%LOCALAPPDATA%\hyperindex\index.db`. **The windows use `%USERPROFILE%\HyperindexDB\<COMPUTER>-<user>-db\index.db`** — pass `--db` to work on the same database as the apps. |
| `--db-cache <MB>` | Database page cache. Default: a quarter of RAM, 64–1024 MB. `0` = SQLite's default. |
| `--progress panel\|bar\|off` | Live display: framed status panel (default), one progress line, or log lines only. Nothing is drawn when output is redirected. |
| `--ascii` | Draw the panel with `+---+` instead of box characters and leave the console code page alone. |

### index scan

```
hypersuite index scan [OPTIONS] [PATHS]...
```

Walks the given folders or drives and records path, size, timestamps and a
BLAKE3 checksum of every file. Only reads.

| Option | Meaning |
|---|---|
| `PATHS` | One or more folders or drives, e.g. `E:\` `D:\Photos`. |
| `--resume` | Continue the most recent interrupted scan with its original paths and options. Paths given alongside select which interrupted scan. |
| `--all-drives` | Scan every mounted local drive. |
| `--include-network` | With `--all-drives`: network drives too. |
| `--follow-symlinks` | Follow symbolic links and junctions (off: avoids loops). |
| `--rehash-all` | Re-checksum every file, ignoring stored values (bit-rot check). |
| `--exclude <name>` | Skip directories with this name everywhere. Repeatable. Windows bookkeeping folders and locked system files are always skipped. |
| `--exclude-path <glob>` | Skip paths matching a glob, e.g. `"**/AppData/Local/Temp/**"`. Repeatable. |
| `--cloud-files skip\|hydrate` | Online-only cloud files: record metadata only (default) or download and hash them. |
| `--threads <n>` | Hashing threads. Default: logical CPUs. |
| `--min-hash-size <bytes>` | Record but don't checksum smaller files. Default 0. |
| `--retries <n>` | Extra attempts after a transient read error. Default 1. |
| `--io-timeout <s>` | Give up on a single file after this many seconds. Default 0 (wait). |
| `--stall-warn <s>` | Warn about a file still being read after this long. Default 60. |
| `--commit-batch <n>` | Files per database transaction. Default 2000. |
| `--flush-interval <s>` | Write at least this often. Default 300. |
| `-q`, `--quiet` | Only the summary line per root. |

```bat
hypersuite index scan E:\ --db D:\index.db
hypersuite index scan --all-drives
hypersuite index scan --resume
hypersuite index scan C:\ --exclude node_modules --exclude-path "**/AppData/Local/Temp/**"
hypersuite index scan \\nas\archive --threads 2 --io-timeout 600 --stall-warn 30
```

### index dupes

Duplicate files across everything indexed. Writes a Markdown report and a
JSON twin; every group names the copy it recommends keeping. Deletes nothing.

| Option | Meaning |
|---|---|
| `--min-size <bytes>` | Ignore smaller files. Default 4096; `0` = all. |
| `-o`, `--out <file>` | Markdown report. Default `hyperindex-report.md`. |
| `--json <file>` | JSON twin. Default: `--out` with `.json`. |

### index doubles

Duplicates at folder level: which folders hold duplicated content, which are
removable as a whole. Reuses a `dupes` report if given or found.

| Option | Meaning |
|---|---|
| `-f`, `--from-report <file>` | Read this `dupes` report (`.md` or `.json`). |
| `--fresh` | Always recompute from the database. |
| `-o`, `--out <file>` | Default `doubles.md`. |
| `--json <file>` | JSON twin. |
| `--min-size <bytes>` | When computing fresh. Default 4096. |

### index enrich

Capture date and offline place name for every photo and its companions
(RAW, XMP, Live-Photo video). Cached; re-runs only process new photos.
`--force` re-derives all.

### index plan / apply / actions — the photo-only library

`plan` writes `plan.md` + `plan.json`: where every photo would go in
`library/photos/<year>/<place>/<date>_<name>`, duplicates, and photos
without a confident date (to `quarantine/`). Nothing is moved.

`apply` copies according to a `plan.json` and verifies every copy:

| Option | Meaning |
|---|---|
| `--plan <plan.json>` | The plan to apply. |
| `--library-root <dir>` | Where the library lives. |
| `--dry-run` | Only show what would be copied. |
| `--undo <job-id>` | Undo one apply run: delete the files it created (never sources). Lists only, unless… |
| `--force` | …this is given. |
| `-o`, `--out` / `--json` | Apply report. Default `apply-report.md`. |

`actions` lists recorded plan runs (`--run <id>` for one run's actions,
`--status <state>`, `--limit <n>`, default 50).

For the complete library of all file types use `hypersuite file` instead.

### index prefilter

Prepares music for [beets](https://beets.io): collapses identical copies to
one and writes a report plus a keep-list (`.txt`, one path per line) for
`beet import`. Options: `--min-size` (default 4096), `-o` (default
`beets-import.md`), `--json`, `--keep-list`.

### index volumes / index stats

`volumes` lists every drive ever indexed (by volume serial), with file count
and size. `stats` shows totals, recent scans and interrupted scans with the
command that started each one.

---

## hypersuite file — Sort

All `file` commands that touch the library need `--db <index.db>` and the
same target folder throughout.

### file plan

```
hypersuite file plan <TARGET> --db <index.db> [OPTIONS]
```

Decides where every indexed photo, music, document and video file would go
under `TARGET`. Writes only a report under `TARGET\.hyperfiler\plans\` and
the planned actions into the database; prints the plan id.

| Option | Meaning |
|---|---|
| `--only <classes>` | Comma-separated: `photo,music,document,video,other`. Default: the first four — `other` only when named. (The Sort window includes Other by default.) |
| `--mirror` | No classification: everything goes to `Archive\<volume serial>\<original path>`. |
| `--entities <file>` | Your vendors, clients and holders (`entities.toml`). |
| `--ocr-pages <n>` | OCR up to n pages of scanned PDFs. |
| `--genres <file>` | Movie → genre table (`genres.toml`). |
| `--model` | Let the language model place documents the rules would send to the Inbox, trained on `--labels`. |
| `--labels <file>` | Labels from `inbox-review`. Default `hyperfiler-labels.jsonl` in the current folder. |

### file review / apply / verify

```
hypersuite file review <PLAN_ID> <TARGET> --db <index.db>
hypersuite file apply  <PLAN_ID> <TARGET> --db <index.db>
hypersuite file verify <TARGET> --db <index.db>
```

- `review` — where one plan's actions stand and why files went to the
  Archive or the Inbox. Read-only.
- `apply` — copies every still-planned action to the target, checks each
  copy against the index's checksum, marks it verified. Never moves or
  deletes a source. Interrupt and re-run freely.
- `verify` — re-checks every verified file in the library against its
  checksum. Read-only; reports missing or changed files.

### file quarantine / purge

```
hypersuite file quarantine <TARGET> --db <index.db> [--plan <PLAN_ID>]
hypersuite file purge <TARGET> --db <index.db> --backup-confirmed "<your note>" [--older-than <days>]
```

- `quarantine` — moves the sources of verified actions to
  `TARGET\.hyperfiler\quarantine\<volume serial>\…`. Deletes nothing. Each
  library copy is re-checked before its source moves.
- `purge` — permanently deletes quarantined files older than `--older-than`
  days (default 30). Requires `--backup-confirmed`, your statement that an
  independent backup of the library exists, recorded as given. Skips any
  file whose library copy no longer checks out. No dry run, no undo.

### file find

```
hypersuite file find --rebuild --db <index.db> [--ocr-pages <n>]
hypersuite file find "car insurance renewal" --db <index.db> [--limit <n>]
```

Semantic search over documents. `--rebuild` reads and embeds every document
(run it first); a query lists the closest matches (default 10).

### file inbox-review / evaluate — teaching the document sorter

```
hypersuite file inbox-review "D:\Documents" [--labels <file>] [--entities <file>] [--limit 50] [--only-inbox] [--ocr-pages <n>] [--model]
hypersuite file evaluate "D:\Documents" [--labels <file>] [--entities <file>] [--ocr-pages <n>] [--model]
```

`inbox-review` shows documents one by one with the rules' suggestion and
records the class you give — the training data for `--model`. Answer:

```
1 Tax   2 Administration   3 Business   4 Family   5 Identity
0 none of these — a manual, an e-book, a README
optionally followed by a type letter: i invoice, c contract, l letter,
s statement, z certificate, f form, o other — e.g. 2i
Enter takes the suggestion, s skips, q stops.
```

Every answer is saved immediately (`hyperfiler-labels.jsonl`); a label
follows the file's content, not its name. Nothing is moved.

`evaluate` measures the rules (and with `--model` the model) against your
labels: how many documents are filed, and how many of those correctly.

---

## hypersuite mail — Outlook to Thunderbird

```
hypersuite mail inspect <PST>
hypersuite mail export <PST> [OPTIONS]
hypersuite mail auto <PST> [OPTIONS]
hypersuite mail backends
```

- `inspect` — folder tree and message counts. Writes nothing.
- `export` — converts into a standalone mbox tree; never touches a
  Thunderbird installation.

  | Option | Meaning |
  |---|---|
  | `--output <dir>` | Default: `<PST name>-thunderbird` next to the PST. |
  | `--overwrite` | Reuse a non-empty output folder. |
  | `--no-keep-errors` | Stop at the first message that fails instead of reporting it and continuing. |
  | `--dry-run` | Show what would be written. |
  | `--root-name <name>` | Put everything under one top-level folder; `""` = the PST's file name. |

- `auto` — guided migration into a Thunderbird profile: checks Thunderbird is
  closed, backs up the profile, converts, validates, then copies into Local
  Folders.

  | Option | Meaning |
  |---|---|
  | `--profile <name or path>` | Asked for if there are several. |
  | `--overwrite` | Allow replacing existing mail folders. |
  | `--dry-run` | Everything except modifying Thunderbird. |
  | `--root-name <name>` | As for `export`. |
  | `-y`, `--yes` | Answer yes to every question (needed without a console). |
  | `--no-start` | Don't start Thunderbird afterwards. |

- `backends` — shows the PST reader in use (built in).

```bat
start /wait hypersuite mail export C:\mail\archive.pst --root-name ""
start /wait hypersuite mail auto C:\mail\archive.pst --root-name "" --yes
```

---

## hypersuite tools

```
hypersuite tools            status of the bundled tools; unpacks them if needed
hypersuite tools --verify   the same, and checks every unpacked file against its SHA-256
hypersuite tools --reset    removes the unpacked copy; it is unpacked again on next use
```

The bundled tools: the multilingual embedding model, PDFium, Tesseract OCR
with German, English, French, Italian, Spanish and Russian, and fpcalc.

---

## Environment variables

hypersuite sets these itself to point at its bundled tools. Set one before
starting hypersuite to use your own copy instead:

| Variable | Points at |
|---|---|
| `TESSERACT_PATH` | `tesseract.exe` |
| `TESSERACT_TESSDATA_DIR` | the folder with `*.traineddata` |
| `PDFIUM_DYNAMIC_LIB_PATH` | the folder with `pdfium.dll` |
| `HYPERFILER_FPCALC_PATH` | `fpcalc.exe` |
| `HYPERFILER_MODEL_DIR` | the embedding model folder (`model.onnx`, `tokenizer.json`, `model_id.txt`) |
