# Privacy Policy — MT Manager

Last updated: 6 October 2026

## Summary

MT Manager does not collect, transmit, sell, or share any personal data. There is
no account to create, no sign-in, no analytics, no advertising, and no telemetry
of any kind. Everything the app stores stays on your own computer.

## Information We Collect

None. MT Manager has no servers, no database, and no mechanism for sending your
information anywhere. We never see your data, because it never leaves your device.

## Information Stored On Your Device

MT Manager saves a small amount of information locally so the app behaves the way
you left it:

- A settings file at `%APPDATA%\MTManager\settings.json`, containing only your
  chosen theme (dark or light), whether automatic update checks are enabled, and
  the last release-notes version you have already seen.
- Windows startup entries, created only for the terminals you explicitly switch
  "autostart" on for. These are standard Windows Run entries stored under your
  own user account.

Both are removed automatically when you uninstall MT Manager.

## Windows Autologon

If — and only if — you choose to turn on Windows autologon, MT Manager asks for
your Windows account password so that Windows can sign itself in after a restart.
This is a standard Windows feature; MT Manager configures it the same way
Microsoft's own Sysinternals Autologon tool does.

What happens to that password:

- It is written to the Windows **LSA private store** as an encrypted secret named
  `DefaultPassword`. This is the same mechanism Windows itself uses for autologon.
- It is **not** written to the registry in plain text. If a plain-text
  `DefaultPassword` value was already there from some earlier tool, MT Manager
  removes it.
- MT Manager keeps **no copy** of the password — not in its settings file, not in
  memory beyond the moment it is stored, and it is never transmitted anywhere.
- To tell you when a stored password has gone stale, MT Manager records only
  **which account** was configured and **when that account's password was last
  changed**, as reported by Windows. Neither the password nor any hash of it is
  part of that record.

Turning autologon off removes the stored secret from your machine.

Please note that autologon is a trade-off you are choosing to make: with it on,
anyone who can physically switch the machine on reaches your desktop without
being asked for a password. It is intended for machines you control, such as a
dedicated trading VPS.

## Access To Your MetaTrader Files

To do its job, MT Manager reads the folder structure of the MetaTrader terminals
installed on your computer and lists the files inside them — their names, sizes,
and modification dates. When you ask it to, it copies, moves, or deletes those
files on your behalf.

MT Manager does not read, collect, or transmit your trading account credentials,
account numbers, balances, positions, order history, or the contents of your
charts and settings. All file operations happen locally on your own computer.

## Internet Connections

MT Manager connects to the internet in only three situations, and never sends any
personal information as part of those requests:

1. **Broker list** — when you open "Install MetaTrader", the app downloads a
   public text file listing available broker terminals from GitHub.
2. **Update check** — when checking for a new version, the app downloads a small
   public JSON file from GitHub, and, if you choose to update, downloads the
   installer for the new version.
3. **Downloads you request** — the Wget Downloader retrieves the exact file at
   the address you supply, and "Install MetaTrader" downloads the installer for
   the broker you select.

All of these are ordinary outbound requests for public files. As with any
internet request, the server on the other end (GitHub, or whichever server you
chose to download from) can see your IP address and standard request information.
That data is handled under those servers' own privacy policies, not ours.

Separately, if the installer detects that .NET Framework 4.8 is missing, it can
open Microsoft's official download page in your browser — but only after asking
you first.

Every other feature of MT Manager works completely offline.

## Third-Party Links

The Donate window opens Trakteer, Sociabuzz, or Ko-fi in your web browser. Those
are independent services with their own privacy policies and terms. MT Manager
does not send them any information about you, and receives nothing back from
them.

## Children's Privacy

MT Manager is a tool for managing trading platform installations and is not
directed at children. It collects no data from anyone, including children.

## Changes To This Policy

If this policy changes, the updated version will be published in the project
repository with a new "last updated" date.

## Contact

Questions about this policy can be raised through the project's issue tracker:

https://github.com/dhimasbagus402/MT-Manager-Windows/issues
