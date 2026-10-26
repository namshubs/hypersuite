# Changelog

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
