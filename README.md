# hypersuite

**Index · Sort · Move your mail** — one Windows program that finds every file
on your drives, sorts them into one clean library, and moves Outlook mailboxes
to Thunderbird.

![The hypersuite launcher](docs/screenshots/launcher-en.png)

| App | What it does |
|---|---|
| **Scan** | Indexes your folders and drives (name, size, dates and a BLAKE3 checksum of every file) into a local database and finds duplicate files and folders — across every drive you have ever scanned, including USB sticks that are not plugged in today. |
| **Sort** | Copies everything indexed into one ordered library — photos by date and place, music by artist and album, documents by kind, videos by title — in four checked steps: Plan → Review → Apply → Verify. The originals stay where they are. |
| **Outbird** | Converts Outlook PST files into Thunderbird mail folders, or puts them straight into your Thunderbird profile (backed up first). |

Everything runs on your computer. hypersuite makes no network connections and
sends nothing anywhere; the document model, OCR (Tesseract, seven languages),
PDF rendering and music fingerprinting all ship inside the one exe.

## Download

Get `hypersuite.exe` from the [latest release](https://github.com/namshubs/hypersuite/releases/latest). No
installer, no runtime to install, no administrator rights needed.

- **Windows 10 or 11, 64-bit.** About 230 MB download; on first start each
  version unpacks about 260 MB of bundled tools into your user profile.
- Each release also has `SHA256SUMS.txt`, the code-signing certificate
  `hypersuite-codesign.cer`, and `third-party-sources.zip` (source code of the
  bundled third-party components under GPL/LGPL).

The exe is signed with a self-signed certificate, so Windows SmartScreen warns
the first time ("Windows protected your PC" → **More info** → **Run anyway**).
[Getting started](docs/getting-started.md) explains how to check the download
and, if you like, how to make Windows trust the signature.

## Documentation

- [Getting started](docs/getting-started.md) — download, verify, first start, update, uninstall
- [Scan](docs/scan.md) — indexing, the database, duplicates, photos, continuing an interrupted scan
- [Sort](docs/sort.md) — the library layout and the Plan → Review → Apply → Verify steps, quarantine and purge
- [Outbird](docs/outbird.md) — Outlook PST to Thunderbird
- [Command line](docs/command-line.md) — every command and option
- [Files, settings and privacy](docs/files-and-settings.md) — what is stored where
- [Troubleshooting](docs/troubleshooting.md)
- Deutsch: [Handbuch](docs/de/handbuch.md) · [Handbuch als PDF](docs/de/hypersuite-handbuch.pdf) · [Kurzanleitung](docs/de/README.md)

## Feedback

- **Found a bug?** [Open an issue](https://github.com/namshubs/hypersuite/issues/new/choose) with the bug report
  form. The version (`hypersuite --version`, or the About page) and the text
  under **Show details** help most.
- **Idea or question?** Use [Discussions](https://github.com/namshubs/hypersuite/discussions) or the feature
  request form.
- **Security problem?** Please don't open a public issue — see
  [SECURITY.md](SECURITY.md).

## About the source code

Development happens on a self-hosted, independent Git server. Only releases
and documentation are published here, so pull requests can't be accepted —
please describe the change in an issue instead.

This is deliberate: it keeps the code base and its core concepts out of
large-scale AI training pipelines, and it keeps the project's direction in
the author's hands.

**Want to contribute or review the code?** Feedback is always welcome. Access
to the source code is for people who share the project's goal — helping users
leave Outlook, clean up Windows and get ready for Linux. It requires four
things (a human, no ties to Big Tech, a record for user rights, a technical
improvement agenda) and an interactive onboarding; see
[CONTRIBUTING.md](.github/CONTRIBUTING.md). Then ask in the "Contributor
access" [Discussion](https://github.com/namshubs/hypersuite/discussions)
category or with the
[Contributor access](https://github.com/namshubs/hypersuite/issues/new?template=contributor_access.yml)
issue form.

## License

[Sustainable Use License 1.0](LICENSE) — free to use for personal,
non-commercial and internal business purposes, and free to share at no
charge for non-commercial purposes; selling hypersuite or offering it
commercially to others is not permitted. hypersuite is not open source.
Version 2.1.3 was released under the Apache License 2.0. **Use at your own risk:** there is no organised support,
and like any software hypersuite may contain errors — see [NOTICE](NOTICE). The bundled third-party components keep their own licenses
(listed in the program under **About**, and in `THIRD-PARTY-NOTICES.md` in
each release).
