# SysBroom

A small, free junk cleaner for Windows 11. It clears caches and temporary files, tells you honestly what it deleted, and collects nothing about you.

## Download

Go to **[Releases → Latest](https://github.com/hightarun/SysBroom-releases/releases/latest)** and download `SysBroom-setup.exe`.

- **Windows 11** (build 22000 or later), 64-bit.
- About 53 MB to download. Everything SysBroom needs is included, so there's nothing else to install first.
- **Installs for your user account only.** No administrator rights, no UAC prompt.

**"Windows protected your PC"?** The installer isn't code-signed yet, so Microsoft SmartScreen may warn you the first time. Click **More info → Run anyway**. Only download SysBroom from this page.

## What it cleans

| Windows | Browsers | Apps | Developer caches (off by default) | System |
|---|---|---|---|---|
| Temporary files (older than 24 hours) | Chrome cache | Discord cache | npm cache | Recycle Bin (off by default) |
| Thumbnail cache | Edge cache | VS Code cache | pip cache | |
| Shader cache | Firefox cache | Steam web cache | NuGet download cache | |
| Crash dumps (off by default) | Brave cache | Teams cache | Gradle cache | |
| | Opera and Opera GX cache | | | |
| | Vivaldi cache | | | |
| | Chromium cache | | | |

Only the browsers, apps and developer tools you actually use are listed. The scan looks for each one's data folder, so it finds a browser wherever it's installed.

You see the size of each item before anything is deleted, and you choose what to clean. Only what's harmless is ticked at first: caches and temporary files that rebuild themselves. Emptying the Recycle Bin is the one step that can't be undone, so it starts unticked, and the Clean button says so when you tick it. Developer caches start unticked too, because your next build downloads them again.

**Never touched:** your documents, Desktop, Downloads, pictures, music and videos, and any browser or app cookies, passwords, history, sign-ins, messages, sessions or saved form data. If an app is open, SysBroom cleans what it safely can and tells you what it skipped. It never closes your programs.

## What it doesn't do

**Runs on your PC · No account · Nothing in the background · Closing it quits it.**

- **No background process.** No tray icon, service or scheduled task. It runs only while its window is open.
- **No telemetry**, analytics, ads or accounts.
- **One network call:** a check of this page for a newer version, at most once a day, which you can turn off. It only tells you; it never downloads or installs anything by itself.

## Uninstall

**Settings → Apps → Installed apps → SysBroom → Uninstall.** It removes the program and its one settings file, and leaves nothing behind.

## Reporting a problem

Open an [issue](https://github.com/hightarun/SysBroom-releases/issues) with your Windows version, the SysBroom version (shown in the window) and what happened.

## Licence

[MIT](LICENSE). This repository holds releases only; the source code is kept separately. The licence doesn't cover the name: forks may not call themselves *SysBroom*.
