# Getting started

## Requirements

- Windows 10 or Windows 11, 64-bit (x64).
- About 500 MB of free space on the system drive: 230 MB for the exe, 260 MB
  for the bundled tools it unpacks on first start.
- Space for the index database: roughly 1 GB per 1.3 million indexed files.
  Scan checks this before it starts and offers another drive if needed.
- Sort needs room for the library it builds — up to the size of everything
  you sort, since it copies.
- No administrator rights, no installer, no .NET, Python or Visual C++
  runtime.

## Download and check

From the [latest release](https://github.com/namshubs/hypersuite/releases/latest) download:

| File | What it is |
|---|---|
| `hypersuite.exe` | the program |
| `SHA256SUMS.txt` | SHA-256 checksums of the release files |
| `hypersuite-codesign.cer` | the certificate the exe is signed with |
| `THIRD-PARTY-NOTICES.md` | licenses of the bundled components |
| `third-party-sources.zip` | source code of the bundled GPL/LGPL components (optional) |

Check that the download is complete and unchanged (PowerShell, in the
download folder):

```powershell
Get-FileHash .\hypersuite.exe -Algorithm SHA256
Get-Content .\SHA256SUMS.txt
```

The two values for `hypersuite.exe` must be identical.

The release notes link the **VirusTotal** report for that same SHA-256, so
you can see what some 70 virus scanners say about exactly this file without
uploading it yourself.

Check the signature:

```powershell
Get-AuthenticodeSignature .\hypersuite.exe | Format-List Status, SignerCertificate
```

The signer is `CN=hypersuite (github.com/namshubs/hypersuite)` with thumbprint
`C7EC126C59C0081863A4467F960C367BA1630C0D` (valid until 2031-10-25). Until your computer trusts this certificate, the
status reads `UnknownError` — the signature is intact, Windows just doesn't
know the publisher.

## First start

1. Put `hypersuite.exe` wherever you like — `Downloads`, a USB stick, a tools
   folder. It does not install anything.
2. Double-click it. **SmartScreen** may say "Windows protected your PC":
   click **More info**, check that the publisher reads *hypersuite (github.com/namshubs/hypersuite)* (or
   *Unknown publisher* if the certificate isn't trusted yet), then **Run
   anyway**. Windows asks only once per version.
3. The **launcher** opens. In the footer, *Unpacking the bundled tools…*
   appears for a few seconds on the first start of each version; then it
   says *Bundled tools ready*.

![Launcher](screenshots/launcher-en.png)

The three cards each open one app in its own window: **Scan**, **Sort** and
**Outbird**. Scan and Sort can run side by side. Clicking a card whose app is
already open brings that window to the front.

`DE | EN` switches the language of every window. It starts from your Windows
display language; your choice is remembered.

### Optional: trust the signature

If you want Windows to show *hypersuite (github.com/namshubs/hypersuite)* as a verified publisher and skip the
SmartScreen warning, import the certificate once (PowerShell or cmd **as
administrator**, in the download folder):

```
certutil -addstore Root hypersuite-codesign.cer
certutil -addstore TrustedPublisher hypersuite-codesign.cer
```

Before you do, compare the certificate's SHA-256 with `SHA256SUMS.txt`.
Trusting a root certificate means trusting everything signed with it; to undo
it, remove "hypersuite (github.com/namshubs/hypersuite)" from both stores in
`certlm.msc`.

## The usual order

1. **Scan** your folders (or whole drives). This only reads.
2. Look at the duplicate reports if you want to clean up first (Scan →
   Advanced).
3. **Sort**: Plan, Review, Apply, Verify. Your originals stay untouched.
4. Optionally, once you have checked the library and have a backup:
   quarantine and later purge the originals (Sort → Advanced → Maintenance).
5. **Outbird** whenever you want to move an Outlook mailbox to Thunderbird —
   it doesn't need a scan.

## Update

Download the new `hypersuite.exe` and replace the old one. Your database,
settings and library are not touched. The new version unpacks its own
bundled tools on first start and removes the previous version's copy.

## Uninstall

1. Delete `hypersuite.exe`.
2. Delete `%LOCALAPPDATA%\hypersuite\` (settings and the unpacked tools).
3. If you no longer need them: the index database (by default
   `%USERPROFILE%\HyperindexDB\`), reports you saved, and the library Sort
   built.

Nothing is written to the registry, Program Files or the system.
