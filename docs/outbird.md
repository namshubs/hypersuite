# Outbird — Outlook mail to Thunderbird

Outbird converts an Outlook data file (`.pst`) into Thunderbird mail folders.
It reads the PST directly — Outlook doesn't need to be installed — and needs
no prior scan.

![Outbird](screenshots/mail-en.png)

## What comes over

- The complete folder tree (Inbox, Sent Items, your own folders …).
- Every message with its original headers where the PST kept them (sender
  and recipients, date, Message-ID, Received lines), plain-text and HTML
  bodies, RTF-only messages converted to text.
- All attachments byte for byte, including mails attached to mails (with
  their own attachments).
- Signed S/MIME messages unchanged, so their signatures still verify.

Outbird moves **mail**. Contacts and calendar entries are not turned into
Thunderbird address books or calendars.

After converting, Outbird checks the result against the PST — every folder,
every message count — and reports any difference.

## Moving a mailbox into Thunderbird

1. **PST file** — Outbird suggests the PST files it finds in Outlook's usual
   folders (`Documents\Outlook Files`, `Documents\Outlook-Dateien`,
   `%LOCALAPPDATA%\Microsoft\Outlook`) and among the files Scan has indexed.
   Or **Browse…**. Once chosen, it shows how many folders and messages the
   file holds.
2. **To** — your Thunderbird profile; Auto picks Thunderbird's default
   profile. **Change…** picks another one.
3. **Close Thunderbird.** Outbird checks this and won't write into a profile
   Thunderbird has open.
4. Tick *I understand this modifies my live Thunderbird profile* and click
   **Move into Thunderbird**, then confirm.

Outbird then:

1. copies the **whole profile** to a backup folder next to it,
   `outbird-backup-<date-time>` (in `%APPDATA%\Thunderbird\Profiles\`);
2. converts the PST into a folder `<PST name>-thunderbird` next to the PST
   file (with a `conversion-report.json`) and validates it — if validation
   fails, the profile is not touched;
3. only then copies the mail folders into the profile's **Local Folders**;
4. starts Thunderbird (unless switched off under Advanced).

The `-thunderbird` folder next to the PST stays as a second copy; delete it
once you are happy with the result. The PST's folder must therefore be
writable and have room for about the PST's size. Thunderbird must be
installed and must have been started at least once (so a profile exists).

The mail appears in Thunderbird under *Local Folders*, by default inside one
folder named after the PST file. If something looks wrong, close Thunderbird
and put the backup folder back in place of the profile folder.

## Export as mbox instead

**Advanced → Destination → mbox folder** writes a standalone folder of
Thunderbird-compatible mbox files without touching any Thunderbird
installation — to look at first, to copy to another computer, or to import
with another mail program. Default location: `<Sort target>\mboxemails\<PST
name>\`. Click **Export as mbox**.

## Advanced

| Option | Meaning |
|---|---|
| Destination | Thunderbird profile (default) or mbox folder. |
| Everything under one top-level folder | On by default; blank name = the PST's file name. Keep it on if several PSTs go into the same profile, so their *Inbox* folders don't merge. |
| Overwrite existing mailboxes/folders | Allow replacing mail folders of the same name. Off by default: Outbird stops rather than overwrite. |
| Dry run | Do everything except write. |
| Start Thunderbird afterwards | On by default. |
| Inspect | Reads the PST's folders and message counts; writes nothing. Use it if a PST can't be opened. |

**Reset Outbird settings to defaults** puts every option back to Auto.

## Several PST files

Repeat for each file. With *Everything under one top-level folder* on, each
PST gets its own folder in *Local Folders*. Sort can also process every PST
it finds in the index in one go — see [Sort → PST files in the
index](sort.md#pst-files-in-the-index).

## Command line

`hypersuite mail inspect | export | auto` — see
[Command line](command-line.md#hypersuite-mail--outlook-to-thunderbird).
