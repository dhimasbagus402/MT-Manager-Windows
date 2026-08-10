[README.md](https://github.com/user-attachments/files/30888070/README.md)
<div align="center">

# MT Manager

**One app to manage every MetaTrader terminal you run.**

Automatically finds every MT4 and MT5 installed on your PC, manages your EAs and
indicators, clears out junk files, duplicates terminals, and downloads EAs
straight from a link — all from a single window.

[![Windows](https://img.shields.io/badge/Windows-7%20SP1%20%7C%2010%20%7C%2011-0078D6?style=flat-square&logo=windows&logoColor=white)](#-system-requirements)
[![Version](https://img.shields.io/badge/version-1-EC3013?style=flat-square)](#)
[![Free](https://img.shields.io/badge/price-free-5ecf3e?style=flat-square)](#)

<img src="Image/main-dark.png" alt="MT Manager main window" width="900">

</div>

---

## Why MT Manager?

If you run more than one MetaTrader account, the small jobs become the tiring
ones. Want to install a single EA across five terminals? Open each data folder
one by one. Wondering why your disk is full? Go dig through `Logs`, `Bases` and
`Tester` yourself. Need a second terminal from the same broker? Reinstall it
from scratch.

MT Manager brings all of it into one place. Your terminals are detected for you,
their contents are laid out by category, and every action is a single click away.

---

## ✨ Features

### Every terminal, found automatically

Hit **Scan MetaTrader** and every installed MT4/MT5 shows up in the sidebar,
grouped by type. Select one to see its details: name, platform, data folder
location, and whether it starts with Windows.

Its contents appear as one clean list with a colour-coded label per category —
**Expert Advisor**, **Indicator**, **Script**, **Log**, **History**, **Ticks**
and **Cache** — along with each file's size and last-modified date.

<img src="Image/main-dark.png" alt="Terminal list and file table" width="820">

### Manage EAs and indicators

Install an EA or indicator into the selected terminal without ever needing to
know which folder it belongs in. Need to remove some? Tick several files and
delete them in one go. **Copy / Cut / Paste** works across terminals too, which
makes putting the same EA on several accounts quick.

<img src="Image/menu-manage-ea.png" alt="Manage EA / Indicator menu" width="820">

### Clear out the junk

MetaTrader quietly piles up logs, price history, tick data and tester caches
that can swallow tens of gigabytes. The **Utility** menu clears them by type, so
you choose exactly what goes without touching your EAs or settings. MetaEditor
opens straight from here as well.

<img src="Image/menu-utility.png" alt="Utility menu" width="820">

### Install, duplicate and uninstall MetaTrader

<img src="Image/menu-add-remove-mt.png" alt="Add / Remove MT menu" width="820">

**Install MetaTrader** gives you a searchable, ready-to-install broker list you
can filter by MT4 or MT5 — pick one and the rest happens on its own. Already have
an installer file of your own? Point it at that instead.

<img src="Image/install-mt.png" alt="Install MetaTrader window" width="620">

**Duplicate MetaTrader** creates a second terminal from the same broker, with a
copy progress bar, and launches it once it's done. Handy when you hold several
accounts at one broker and want each to have its own terminal.

<img src="Image/duplicate-mt.png" alt="Duplicate MetaTrader window" width="620">

### Download EAs straight from a link

Paste a URL (or a full `wget` command) into the **Wget Downloader** box and the
file downloads with a progress bar. `.zip` files are extracted automatically the
moment they finish, so an EA is ready to use without a detour through File
Explorer.

### Start automatically with your PC

Every terminal gets its own **autostart** switch. Turn it on and that terminal
launches whenever Windows boots — ideal for a VPS that has to stay online. If
you ever uninstall MT Manager, every autostart entry it created is removed for
you.

### Dark and light themes

One click switches the theme, and the whole app follows instantly — title bar
included.

<img src="Image/main-light.png" alt="Light theme" width="820">

### Notifications that stay out of the way

Messages appear briefly and fade on their own. No more dialog boxes to dismiss
every time something finishes.

<img src="Image/toast.png" alt="Self-dismissing notification" width="820">

### Always up to date

MT Manager checks for updates, downloads, installs and restarts itself — you
just press one button. Every release comes with notes you can read any time from
**What's New**.

<img src="Image/whats-new.png" alt="What's New window" width="620">

---

## 💻 System Requirements

| | Minimum |
|---|---|
| **Operating system** | Windows 7 SP1 or newer — Windows 8, 8.1, 10 and 11 fully supported (32-bit and 64-bit) |
| **.NET Framework** | Version 4.8. Already included in Windows 10 (May 2019 update) and later; the installer will tell you and point you to Microsoft's official download if it's missing |
| **MetaTrader** | MT4 and/or MT5 installed normally. **Portable** installations are not detected |
| **Disk space** | About 10 MB for the app |
| **RAM** | Nothing special — this is a lightweight app |
| **Administrator rights** | **Not required.** MT Manager installs per user. Administrator is only needed if you duplicate a terminal that lives inside `Program Files` |
| **Internet connection** | Only needed for the broker list, update checks and the Wget Downloader. Everything else works offline |

---

## 📥 Installation

1. Download `MTManager-Setup-1.exe` from the [Releases](../../Release) page.
2. Run the installer and follow it through.
3. Open MT Manager, press **Scan MetaTrader**, and your terminals appear.

There's nothing to configure afterwards.

---

## ❤️ Support This Project

MT Manager is free for anyone to use. If it saves you time, any support at all
goes a long way toward keeping it developed.

<img src="Image/donate.png" alt="Donate dialog" width="480">

<div align="center">

[![Trakteer](https://img.shields.io/badge/Trakteer-EC3013?style=for-the-badge)](https://trakteer.id/dhimas_bagus4/tip)
[![Sociabuzz](https://img.shields.io/badge/Sociabuzz-EC3013?style=for-the-badge)](https://sociabuzz.com/dhimasbagus402/tribe)
[![Ko--fi](https://img.shields.io/badge/Ko--fi-EC3013?style=for-the-badge)](https://ko-fi.com/dhimasbagus)

</div>

---

## ❓ FAQ

**Does MT Manager change my trading settings or accounts?**
No. It only manages files and folders that belong to your terminals — installing,
copying and deleting EAs and indicators, and clearing logs and caches. Your
accounts, charts and trading settings are never touched.

**Why doesn't my terminal show up when I scan?**
MT Manager reads terminals that were installed normally. MetaTrader running in
**portable** mode keeps its data inside its own program folder, so it isn't
detected.

**Will my MetaTrader data be deleted if I uninstall MT Manager?**
No. Only MT Manager's own things are removed — its settings and any autostart
entries it created. Your MetaTrader data folders are left untouched.

**Is this paid software?**
No, it's completely free.

---
