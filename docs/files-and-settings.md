# Files, settings and privacy

## Privacy

hypersuite works entirely on your computer:

- It makes **no network connections** — no updates, no telemetry, no
  accounts, no downloads. The language model, OCR, PDF renderer and music
  fingerprinter all ship inside the exe.
- Photo places are looked up in a built-in offline city database; GPS data
  never leaves your computer.
- The only way hypersuite causes network traffic is indirectly: scanning
  online-only cloud files with *download and hash* makes OneDrive (or another
  sync client) download them, and scanning a network drive reads over the
  network.

## What is stored where

| What | Where | Notes |
|---|---|---|
| Settings | `%LOCALAPPDATA%\hypersuite\settings.json` | Language, folder selection, database, target, options; *Recently used* databases. Delete it to start from defaults. |
| Bundled tools | `%LOCALAPPDATA%\hypersuite\runtime\<version id>\` | About 260 MB, unpacked once per version, checked against SHA-256. Older versions' copies are removed automatically. |
| Index database (apps) | `%USERPROFILE%\HyperindexDB\<COMPUTER>-<user>-db\index.db` | Or wherever you chose. Holds paths, sizes, dates and checksums of indexed files, photo dates/places, Sort's plans and actions, document embeddings for search. **No file contents.** |
| Index database (command line) | `%LOCALAPPDATA%\hyperindex\index.db` | Default when `--db` isn't given. |
| Scan reports | `Documents\hypersuite\` | Duplicate reports, photo plans, beets keep-lists. Changeable under Scan → Advanced. |
| Library | `<X>:\hypersuite\` | Or the target you chose. |
| Sort plans and reports | `<target>\.hyperfiler\plans\` | |
| Quarantine | `<target>\.hyperfiler\quarantine\` | Originals moved aside by *Quarantine*. |
| Outbird conversion | `<PST name>-thunderbird\` next to the PST | When moving into Thunderbird; plus `conversion-report.json`. |
| Thunderbird backup | `%APPDATA%\Thunderbird\Profiles\outbird-backup-<date-time>\` | A full copy of the profile, made before Outbird writes into it. |
| Document labels | `hyperfiler-labels.jsonl` in the current folder | Only if you use `hypersuite file inbox-review`. |

Nothing is written to the registry, `Program Files`, or anywhere outside these
places.

The index database is an ordinary SQLite file. It contains the names and
locations of your files, so treat it like a directory listing of your drives:
don't share it if those names are private.

## Database size

Roughly 736 bytes per indexed file — about 1 GB per 1.36 million files —
plus document embeddings if you use search. Scan checks for room before it
starts.

While hypersuite runs, SQLite keeps `index.db-wal` and `index.db-shm` next to
the database. They are folded back in when the last program using the
database closes. If a process was killed, they may stay; open the database
once in Scan and close it again.

## Settings file

`settings.json` is plain JSON and is rewritten by the apps. Each app process
writes back only its own section, so Scan, Sort and Outbird can be open at
the same time. Values marked `"mode": "auto"` are recalculated at every start;
`"mode": "manual"` values are kept as they are.

To reset one app: **Reset … settings to defaults** under its Advanced section.
To reset everything: close hypersuite and delete `settings.json`.
