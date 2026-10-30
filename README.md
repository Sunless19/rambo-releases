# RAMbo

A lightweight Windows memory cleaner. Formerly called SelfMemReduct. It frees cached and idle RAM, shows what is using your memory, and lives quietly in the tray.

**[⬇ Download the latest version](https://github.com/Sunless19/rambo-releases/releases/latest)**

## Features

- Live dashboard: RAM gauge, committed memory, standby cache and a 3-minute history graph
- One-click cleaning, a global hotkey (Ctrl+F1 by default) and a tray icon showing your current RAM %
- Auto-clean when RAM goes over a percentage you set, and/or on a timer
- Processes view: see which apps use the most RAM, then trim or end them
- Safe defaults: options that can cause stutter are off and clearly marked
- **No internet access, no telemetry, no ads.** The app contains no network code at all.

## Install

1. Download **`RAMbo-Setup-<version>.exe`** from the [latest release](https://github.com/Sunless19/rambo-releases/releases/latest).
2. Run it and click **Install**. Windows asks for administrator rights, which are needed to clear system memory lists.
3. Find it in the Start menu as **RAMbo**.

**"Windows protected your PC"?** The installer isn't signed with a paid code-signing certificate, so SmartScreen warns about it. Click **More info → Run anyway**.

**Portable version:** download `RAMbo-<version>-portable.zip`, unzip it anywhere and run `RAMbo.exe`. There's nothing to install.

**Uninstall:** go to Windows **Settings → Apps → RAMbo → Uninstall**.

**Upgrading from SelfMemReduct 1.1.0?** Just run the RAMbo installer. It carries over your settings, log and start-with-Windows choice, and removes the old app.

**Silent install** (for IT and scripts): `RAMbo-Setup-<version>.exe /S`

## Requirements

Windows 10 or 11, 64-bit. It uses the .NET Framework 4.8 that's already built into Windows.

## Verify your download

Each release lists SHA-256 checksums. To check yours, run this in PowerShell:

```powershell
Get-FileHash .\RAMbo-Setup-1.2.0.exe -Algorithm SHA256
```

## A note on "freeing RAM"

Windows deliberately uses spare RAM as a cache, because unused RAM is wasted RAM. Cleaning helps when something is genuinely short on memory, such as a game stuttering because RAM is full. It doesn't make a healthy PC faster.

---

This repository only hosts releases. The source code is private.
