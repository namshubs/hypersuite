# Changelog

## 2.2.1 — 2026-11-06

**Local AI – no data in, no data out.** To sort documents, hypersuite uses one
local AI model: **multilingual-e5-small** (Microsoft Research, MIT licence), a
small embedding model – not a chatbot, it writes no text. It is built into the
exe and runs on your own processor. hypersuite is hardened by design: it has no
network function at all – no downloads, no updates, no telemetry, no cloud, no
account. Nothing comes in from outside and nothing that was read goes out;
checked in the source code and measured during a run with OCR and AI: zero
network connections. **The AI learns nothing:** the model is never trained or
changed, so after a run it knows nothing about your documents. What Plan has
read stays only in a local cache file on your own disk, which you can delete at
any time. Appendix A of the user manual explains how the AI is built in and how
to check this yourself or enforce it with a firewall rule.

- **Sort → Plan shows where it is.** Step x of n (photos, music, documents,
  videos, other data, saving the plan), a bar with files done and time left,
  the file being read right now, and a note when one file takes long.
- **Plan continues instead of starting over.** What Plan has read (text,
  OCR, AI) is kept in a cache (`%LOCALAPPDATA%\hyperfiler\plan-cache.db`, by
  file content). After a cancel, a crash or a power cut, Plan skips what it
  already read; a second Plan with other settings is much faster too.
- **Plan reads several documents at once.** A speed slider in the Plan step
  (1 up to all cores, default half) — it can be moved while Plan runs. A
  speedometer shows the computer's CPU load and Plan's share of it. On a
  test with scanned PDFs, 4 at once was 3× faster, 8 at once 4×.
- **Time limit per document** (default 120 s, under Advanced): a document
  that takes longer is copied unchanged into the Archive and listed in the
  report, instead of holding up the whole plan.
- **Fix: the AI step could crash a large Plan at the very end.** All
  documents were embedded in one block, untruncated. Now in small batches,
  cut to the model's 512 tokens, and only for documents the AI can actually
  help with; without your own labels it is skipped entirely.
- Verify shows a progress bar too.

## 2.2.0 — 2026-11-05

- **Scan: drives one by one.** Every local drive — fixed and removable (USB
  docks) — can be ticked on its own, besides the folders.
- **Scan: "Don't scan" list.** Folders to leave out with everything below
  them, plus suggestions that are on by default: the Sort target,
  `hypersuite` folders, the database folder, rescue folders and photo
  libraries of earlier runs. A suggestion a scanned folder lies in is not
  applied, so the rescue folder itself can still be scanned.
- **Forensic mode** for drives that drop out after a while (heat, USB dock):
  Scan lists metadata only, saved folder by folder, and continues where it
  stopped — after a drop-out it cools down, waits for the same drive (under
  any letter), optionally restarts its USB device, and carries on by itself.
  Sort then offers **Rescue files**: copies them unchanged into
  `<target>\_rescue\…`, smallest first, skips files that hang instead of
  waiting, pauses before the drive is expected to fail again, and can be
  paused and continued at any time.
- Command line: `index scan --forensic`, `--exclude-dir`, `index rescue`.

## 2.1.7 — 2026-10-26

- The exe's file properties (*Copyright*) name the Sustainable Use License
  1.0; 2.1.4 to 2.1.6 still said Apache License 2.0 there.
- No functional changes.

## 2.1.6 — 2026-10-26

- Outbird opens PST files strictly read-only. Before, the PST reader also
  took a write handle whenever Windows allowed it (it never wrote through
  it); now there is none.
- README: *What it does to your files* — what each step reads, writes, moves
  or deletes, how duplicates are decided, and where the dry runs are.
- Release notes link the VirusTotal report of the release's `hypersuite.exe`.
- License section states plainly: source-available on request, not open
  source, and why 2.1.3 was Apache 2.0.

## 2.1.5 — 2026-10-26

- `THIRD-PARTY-NOTICES.md` (also under **About**) opens with hypersuite's own
  license — the Sustainable Use License 1.0, not the Apache License 2.0 as
  2.1.4 still said there — followed by why the source code is not published,
  how to take part, and the use-at-your-own-risk notice.
- Contributing: the requirements for source access and the contributor
  agreement are in `.github/CONTRIBUTING.md` and
  `.github/CONTRIBUTOR-AGREEMENT.md`; the German handbook describes them.
- No functional changes.

## 2.1.4 — 2026-10-26

- **License: Sustainable Use License 1.0** (`LICENSE`) instead of the Apache
  License 2.0: free for personal, non-commercial and internal business use,
  and free to share at no charge for non-commercial purposes; selling
  hypersuite or offering it commercially to others is not permitted.
  hypersuite is not open source. Copies of 2.1.3 keep the Apache License 2.0.
- README, handbook and `NOTICE` explain why the source code is not published
  and how to ask for contributor access (new issue form *Contributor access*).
- No functional changes.

## 2.1.3 — 2026-10-25

- **License: Apache License 2.0** (`LICENSE`), with the copyright and a
  "use at your own risk" notice in `NOTICE` — both shown under About.
  Replaces the hypersuite License, version 1.
- New signing certificate: the publisher is now
  `hypersuite (github.com/namshubs/hypersuite)` (thumbprint
  `C7EC126C59C0081863A4467F960C367BA1630C0D`). If you trusted the previous
  certificate, import the new `hypersuite-codesign.cer`.
- Fixed: **Sort → Make plan failed** with `UNIQUE constraint failed:
  actions.plan_run, actions.file_id` when the index held `.mov` files (a
  `.mov` counted as Live-Photo companion and as video) or XML photo sidecars
  (`.xmp`, `.aae` also counted as documents). Every file now belongs to one
  class: a `.mov` next to a photo of the same name is part of that Live
  Photo, any other `.mov` is a video.
- PDFs that a parser can't read no longer print a "panicked at … bad length
  of hexstring" message for every file; they are reported as unreadable and
  go to the Inbox, as before.
- Engines: hyperindex 0.103.1, hyperfiler 0.18.2, Outbird 1.0.0.

## 2.1.2 — 2026-10-25

First public release.

- New license: **hypersuite License, version 1** — free to use, privately and
  commercially, without warranty (see `LICENSE`). Replaces the earlier
  proprietary license.
- Releases now include `third-party-sources.zip`, the complete source code of
  the bundled GPL/LGPL components (libjbig, libidn2, libintl, libiconv,
  libunistring, Chromaprint/FFmpeg in fpcalc).
- Fixed: a `settings.json` saved with a byte-order mark (as Notepad or
  Windows PowerShell 5 write it) was ignored, so every setting fell back to
  its default. It is read correctly now.
- `hypersuite tools --help` prints the tool's usage instead of "unknown
  option".
- Command-line help of `hypersuite file` cleaned up (examples use a neutral
  database path; no references to internal design documents).
- The exe no longer contains paths of the build machine.
- Engines: hyperindex 0.103.1, hyperfiler 0.18.1, Outbird 1.0.0.

## 2.1.0 — 2026-10-24

- **Open an existing database** in Scan and Sort: *Open existing…*, *New…*,
  *Recently used…* (last five). The line under the path shows files, drives
  and the last scan; a file that isn't an index database is shown in red.
- Opening a database takes over the folders and options of its last scan.
- **Continue an interrupted scan**: a card shows what is left to do;
  *Continue* resumes it without re-reading finished files.

## 2.0.0 — 2026-10-24

- New window design: a **launcher** with three apps — **Scan**, **Sort** and
  **Outbird** — each in its own window; Scan and Sort can run side by side.
- **Automatic defaults** (● Auto), worked out at every start: user folders to
  scan, database location, library target on the drive with the most free
  space, Thunderbird profile. Changed values turn *Manual* and are kept.
- Scan counts files first, checks room for the database (and proposes another
  drive if needed), and shows progress with remaining time.
- Sort as four steps: Plan → Review → Apply → Verify.
- Outbird finds PST files in Outlook's folders and in the index.
- German and English interface (`DE | EN`), starting from the Windows display
  language.

## 1.0.0 — 2026-10-19

- First version: hyperindex (indexing, duplicates, photo enrichment),
  hyperfiler (library: plan, apply, verify, quarantine, purge, semantic
  search) and Outbird (Outlook PST to Thunderbird, rewritten in Rust) in one
  Windows exe with a GUI and their full command lines.
- Everything bundled: multilingual document model, PDFium, Tesseract OCR
  (German, English, French, Italian, Spanish, Russian), fpcalc.
