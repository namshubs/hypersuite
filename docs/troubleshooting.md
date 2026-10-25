# Troubleshooting

### "Windows protected your PC" when starting hypersuite

SmartScreen doesn't know the self-signed publisher yet. Click **More info**
→ **Run anyway**. To make Windows trust it permanently, see [Getting
started → Trust the signature](getting-started.md#optional-trust-the-signature).
Check the download's SHA-256 first.

### The launcher says "Tools missing – see Tools"

The bundled tools couldn't be unpacked or a file was damaged (for example by
antivirus software or a full disk). Open **Tools** in the launcher footer and
click **Unpack again**, or run `hypersuite tools --reset` and start hypersuite
again. Needs about 260 MB free in `%LOCALAPPDATA%`.

### Nothing appears when I run hypersuite in cmd

The exe is a windowed program, so cmd doesn't wait for it and its output
lands after the next prompt. Use `start /wait hypersuite …` in cmd and batch
files, or `hypersuite … | Out-Host` in PowerShell.

### A scan seems stuck on one file

Usually a cloud file that the sync client can't deliver, a dying disk or a
slow network share. The log (**Show details**) names any file still being
read after 60 seconds. Options: exclude that folder, leave *Online-only
files* on **skip**, or on the command line use `--io-timeout` and
`--threads 2` for slow sources. Stopping and **Continue** later loses
nothing.

### The scan was interrupted

Open Scan: it shows **The last scan was interrupted** — click **Continue**.
Files already indexed are not read again. On the command line:
`hypersuite index scan --resume`.

### "Not a hyperindex database, or not readable"

The chosen file isn't an index database, or another program has it locked.
Choose the right file with **Open existing…**, or **New…** to create one.

### Sort says "Scan first"

Sort works from the index. Scan your folders first, or point Sort at an
existing database (**Pick an existing index…**).

### Many documents land in Docs\Inbox

The Inbox is where documents go when the rules aren't confident — by design,
nothing is guessed. To file more of them:

- Add your vendors, clients and family members to `entities.toml`
  (Sort → Advanced).
- Switch on OCR pages for scanned PDFs.
- Label some documents with `hypersuite file inbox-review` and switch on
  *AI document sorting*.

### Files went to Archive instead of Photo/Music/Video

A file without usable tags or date, or one the index hasn't checksummed yet
(for example online-only cloud files), is copied to `Archive\<volume
serial>\<original path>` instead of being guessed at. For photos, run
**Enrich photos** in Scan before planning. For cloud files, scan with
*download and hash*.

### Apply fails for some files

A source that changed after planning, or that is no longer reachable (drive
unplugged), fails instead of being copied wrongly. Plug the drive in or scan
again, make a new plan, and apply it. Everything already copied is kept.

### Outbird: "Thunderbird appears to be running"

Close Thunderbird completely (also from the notification area) and try again.

### Outbird: "… already exists in the Thunderbird profile"

The profile already has a mail folder with that name — typically from an
earlier run. Keep *Everything under one top-level folder* on (or give it a
different name), choose another profile, or switch on *Overwrite* if you
really want to replace it.

### Outbird: no Thunderbird profile found

Install Thunderbird and start it once so it creates a profile. Or export as
an mbox folder (Advanced → Destination).

### Reporting a problem

[Open an issue](https://github.com/namshubs/hypersuite/issues/new/choose)
with:

- the version (`hypersuite --version`, or **About** in the launcher),
- your Windows version,
- what you did and what happened,
- the text under **Show details** (remove any file names you consider
  private).
