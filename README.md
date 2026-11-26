<p align="center">
  <img src="Trialux-Presenter-logo-on-charcoal.png" alt="Trialux Presenter" width="640">
</p>

# Trialux Presenter

**Trial exhibit presentation for Windows.** Trialux Presenter shows your exhibits to the jury on a second screen while you work from your own: highlight, call out, redact, stamp and point, without the jury ever seeing your menus, notes or the next exhibit.

Trialux Presenter was previously called **Trialux**. Your cases, settings and license carry over.

Website: **[gettrialux.com](https://gettrialux.com)**

This repository holds **official Trialux Presenter releases and update information only**. Trialux Presenter is commercial software; its source code is not published here.

## Download

<!-- release-info:start (updated by release.ps1) -->
**Latest version: 2.3.4** (November 25, 2026). [Download Trialux-Presenter.exe](https://github.com/legallytom/trialux-presenter-releases/releases/latest/download/Trialux-Presenter.exe) or see the [Releases page](https://github.com/legallytom/trialux-presenter-releases/releases/latest).
<!-- release-info:end -->

Save **Trialux-Presenter.exe** to your **Desktop** and double-click it there to open Trialux Presenter. On the Desktop it is always one double-click away, and Trialux Presenter can update itself there. No long installation needed. Avoid putting it in Program Files, where Windows won't let it update itself.

At its first update, the file is renamed to **Trialux Presenter.exe** (a download can't have the space in its name). Shortcuts on your Desktop and in the Start menu follow it. If you pinned it to the taskbar or Start and the pin stops working, pin it again. A file you renamed yourself keeps your name.

## What it does

- **Present to the jury** on a second display or projector while you keep working on your own screen. Pause, freeze, side-by-side, call-outs and a laser pointer.
- **Mark up exhibits**: highlighting that snaps to the words, pen, arrows and shapes, redactions, and exhibit stamps in the usual sticker styles.
- **Organize a case**: exhibit numbers, groups, rulings (admitted or denied, with a warning before a denied exhibit reaches the jury), and search inside every exhibit, including scanned pages.
- **Documents, photos, audio and video** in one exhibit list.
- **Export**: marked PDFs, with redacted text removed for good and the rest kept searchable; a Word exhibit list; snapshots of what the jury saw.

## System requirements

- Windows 10 (version 2004 or later) or Windows 11, 64-bit
- A second display, projector or TV for presenting (optional for preparing)
- Internet access to activate a license, at least once every 21 days to confirm it (Trialux Presenter checks weekly by itself), and for updates. Otherwise it works offline, including in a courtroom with no connection

## Trial and license

Trialux Presenter runs as a full **7-day trial** from the first time it opens. In the last 3 days it reminds you once a day. When the trial ends, it locks until a license key is entered.

To activate, choose **Help > License**, paste your license key and choose **Activate**. The computer must be online for this step. After that:

- **Trialux Presenter works offline,** including in a courtroom with no connection.
- **It confirms the license about once a week** by itself whenever the computer is online.
- **If it can't confirm for 21 days, it locks** until the computer is connected. Connect your laptop before a trial or hearing, not at the courthouse.
- **If it locks when you need it** (no connection, or a renewal that hasn't gone through), the license window offers **Emergency 72 Hours**: full use without the internet, once per license term on each computer.

A license runs for **one year** and includes every update released during that time. To keep using Trialux Presenter after that, renew the license. Reminders start 30 days before it ends. Once it's renewed, choose **Help > License > Check Now**.

Each license covers a set number of computers. To move to a new computer, choose **Help > License > Deactivate This Computer** on the old one first, which frees its seat.

Activation and the weekly check send the license server your license key, a fingerprint of the computer (a one-way hash, not the Windows ID itself), the computer's name, and the Trialux Presenter version. No case files, exhibits or other content are ever sent.

Your exhibits are your own files, so they stay usable in other programs even while Trialux Presenter is locked.

To buy or renew a license, or for any question: [support@gettrialux.com](mailto:support@gettrialux.com)

## Updates

Trialux Presenter checks this repository for a new version once a day, if allowed in Edit > Preferences, and tells you when one is available. To install it, choose **Help > Check for Updates**. It downloads the new version, checks it and restarts. Nothing is installed without your say-so, and it never updates while you are presenting.

Every release includes:

| File | What it is |
| --- | --- |
| `Trialux-Presenter.exe` | The program |
| `manifest.json` | The version, download address and SHA-256 fingerprint of the program |
| `manifest.json.sig` | A digital signature of `manifest.json` |

Trialux Presenter only accepts an update whose `manifest.json` is signed with the publisher's key, and whose download matches the fingerprint in that signed manifest.

### Checking a download yourself

In PowerShell, in the folder where you saved it:

```powershell
Get-FileHash .\Trialux-Presenter.exe -Algorithm SHA256
```

The result should match the `sha256` value in that release's `manifest.json`.

## Support

Email **[support@gettrialux.com](mailto:support@gettrialux.com)** with questions, problems, purchases and renewals, or visit **[gettrialux.com](https://gettrialux.com)**.

When reporting a problem, include your Trialux Presenter version (Help > About) and, if possible, the log file at `%LOCALAPPDATA%\Trialux\log.txt`.

## License

Copyright © 2026 JADTEB, LLC, an Iowa limited liability company. All rights reserved.

Trialux Presenter is licensed, not sold. Your use of it is governed by the [Trialux Presenter End User License Agreement](EULA.txt), which you accept when it first opens and can read at any time in **Help > License Agreement**. Nothing in this repository grants any right to copy, modify or distribute Trialux Presenter.

Trialux Presenter includes open-source components, each used under its own license. The full notices are in the program under **Help > Open-Source Licenses**. Those projects and their authors don't endorse Trialux Presenter.

Microsoft, Windows and Word are trademarks of the Microsoft group of companies.
