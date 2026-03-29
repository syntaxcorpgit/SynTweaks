# SynTweaks

> System Optimizer & Fixer v2.0 by SyntaX

![Version](https://img.shields.io/badge/version-2.0.0-cyan)
![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011-0f172a)
![.NET](https://img.shields.io/badge/.NET-8.0-512bd4)
![Status](https://img.shields.io/badge/status-active-16a34a)
![License](https://img.shields.io/badge/license-private%20project-b91c1c)

SynTweaks is a private Windows optimization, repair, cleanup, diagnostics, and debloat toolkit built for power users, gamers, technicians, and internal testers who want one console application to handle system tuning and troubleshooting in one place.

It includes:

- an SSH-style branded startup experience
- arrow-key navigation across all menus
- performance, privacy, network, app, registry, and service tuning
- repair modules for common Windows hardware and software issues
- cleaner modules for temp files, caches, and junk
- optional AI-assisted system analysis
- built-in logs, restore point prompts, and Discord reporting tools

## Private Project Notice

This repository is **not open source**.

- Source code is private and proprietary.
- Redistribution, reuse, or republishing is not permitted unless explicitly authorized by the owner.
- Public contributions, forks, and third-party redistribution are not part of this project workflow.
- Support, feedback, bug reports, and feature requests should go through approved private channels or the built-in `Report Center`.

## Quick Start

If you are using SynTweaks for the first time:

1. Launch `SynTweaks.exe` as Administrator.
2. Let the SSH-style startup finish and wait for the main menu.
3. Use `Up Arrow` and `Down Arrow` to move through the menu.
4. Press `Enter` to open a module.
5. Press `Esc` to go back.
6. Start with `Essential Tweaks`, `Privacy Guard`, `Cleaner Suite`, or `Tools & Diagnostics`.
7. Use `Advanced Tweaks`, `Registry Manager`, `Service Manager`, and `App Debloater` more carefully.
8. Allow restore point creation when prompted for higher-impact actions.

## What SynTweaks Is Built For

SynTweaks is meant to help users:

- reduce Windows background clutter
- tune gaming-related behavior
- clean caches, temp files, and junk
- disable unnecessary apps, services, or startup behavior
- troubleshoot broken Windows components
- repair audio, display, driver, input, and shell issues
- review system diagnostics before reporting problems
- analyze health and crash patterns with optional AI support

## Main Modules

| Module | Purpose |
|---|---|
| `Essential Tweaks` | Baseline Windows optimizations and common quality-of-life improvements |
| `Advanced Tweaks` | Deeper system changes for experienced users |
| `Gaming Optimizer` | CPU, GPU, storage, network, and latency-oriented gaming tweaks |
| `Privacy Guard` | Telemetry, tracking, diagnostic, and privacy controls |
| `Network Optimizer` | DNS changes, stack resets, IPv4/IPv6 controls, and adapter tuning |
| `Service Manager` | Startup mode control, service disabling, restoration, and exports |
| `App Debloater` | Removal of bundled apps, gaming extras, and browser/platform clutter |
| `Feature Control` | Explorer and Windows feature toggles |
| `Registry Manager` | Registry backups, imports, exports, and common registry presets |
| `Tools & Diagnostics` | General helpers, system information, and diagnostic utilities |
| `Fix Center` | Dedicated repair menus for Windows, drivers, audio, display, keyboard, and mouse issues |
| `Cleaner Suite` | Temp/cache cleanup and junk file sweeping |
| `AI Analyzer` | Offline or OpenRouter-powered system analysis and crash-log review |
| `About SynTweaks` | Product overview, version info, and developer credits |
| `Report Center` | Bug, crash, performance, and feature request reporting |

## Navigation Guide

SynTweaks is designed to be used without typing in most places.

- `Up Arrow` and `Down Arrow` move between options
- `Enter` confirms the current option
- `Esc` returns to the previous menu
- confirmation prompts use the same arrow-driven interaction
- text entry is only enabled when needed, such as for report text or AI key entry

The UI keeps the cursor hidden during animation and menu rendering, then briefly re-enables it for text fields.

## Recommended First Session

For a safe and practical first run:

1. Open `Tools & Diagnostics` and review the machine state.
2. Apply a few `Essential Tweaks`.
3. Open `Privacy Guard` and choose only the privacy changes you actually want.
4. Run `Cleaner Suite` to remove temp and cache buildup.
5. If this is a gaming machine, continue into `Gaming Optimizer`.
6. Leave `Advanced Tweaks`, `Registry Manager`, and `Service Manager` for later unless you already know what you need.

## Fix Center Overview

The `Fix Center` contains separate repair modules for:

- `Windows Common Fixer`
- `Driver Fixer`
- `Display Fixer`
- `Sound Fixer`
- `Microphone Fixer`
- `Headset Fixer`
- `Keyboard Fixer`
- `Mouse Fixer`

Examples of issues SynTweaks can help address:

- Windows Update failures
- Explorer crashes or sluggish shell behavior
- slow boot and shutdown behavior
- missing DLL or runtime issues
- Microsoft Store launch issues
- GPU detection or refresh rate issues
- black screen, flickering, HDR, and display routing issues
- audio stuttering, missing output devices, or HDMI audio issues
- microphone privacy or Discord/game microphone issues
- keyboard lag, wrong layout behavior, or disabled keys
- mouse acceleration, lag, disconnects, and double-click problems

## Cleaner Suite Overview

The `Cleaner Suite` covers both temporary cleanup and broader junk removal.

It includes cleanup routines for:

- user temp folders
- Windows temp folders
- prefetch data
- browser caches
- Discord, Teams, Zoom, Spotify, Steam, Epic Games, and similar caches
- crash dumps and Windows Error Reporting files
- thumbnails, icon cache, and font cache
- old files, zero-byte files, and empty folders
- recycle bin cleanup
- duplicate and large file analysis helpers
- old restore point cleanup helpers
- WinSxS and delivery optimization cleanup helpers

## AI Analyzer

SynTweaks supports two AI workflows:

- `Run AI Health Analysis`
- `Analyze Crash Logs`

The AI system can:

- collect a live system snapshot
- inspect CPU, RAM, disk, and recent errors
- read applied tweak history from logs
- suggest automation-safe actions
- analyze crash summaries
- optionally trigger supported auto-fix actions

### Online and Offline Modes

SynTweaks can work in:

- `Offline mode`
  Uses local fallback analysis and does not require an API key.

- `Online mode`
  Uses OpenRouter for richer AI responses and recommendations.

### OpenRouter API Key

If you want online AI analysis:

- SynTweaks will prompt for an OpenRouter API key
- the key is stored in `%APPDATA%\SynTweaks\config.json`
- the stored key is encrypted for the current Windows user
- if no key is provided, the program falls back to offline analysis

## Report Center

The `Report Center` can send:

- bug reports
- crash reports
- performance reports
- feature requests

Each report can include:

- system information
- application version
- recent SynTweaks log lines
- recent Windows Application event errors

There is also a local diagnostics preview so users can see what information is available before sending a report.

### Discord Reporting

The report system can use a Discord .

It supports:

- a built-in sender value inside the codebase

If the webhook is unavailable, SynTweaks fails gracefully and explains what is missing.

## Logs, Config, and Stored Data

SynTweaks stores application data under:

- `%APPDATA%\SynTweaks\`

Important locations:

- logs folder: `%APPDATA%\SynTweaks\logs\`
- daily log file format: `syntweaks_YYYY-MM-DD.log`
- fallback log file: `syntweaks_fallback.log`
- AI configuration file: `%APPDATA%\SynTweaks\config.json`

Some repair and diagnostic tools also export reports or inventories to the Desktop.

## Safety and Risk Notice

SynTweaks is a power tool. Some actions modify:

- the Windows registry
- service startup modes
- power plans
- DNS configuration
- IPv4/IPv6 behavior
- installed or provisioned applications
- shell and Explorer behavior
- hosts file entries

Before using deeper modules:

- run the app as Administrator
- read each action label before confirming it
- create restore points when prompted
- avoid bulk-running advanced actions unless you know the effect
- reboot when a module recommends it

Be especially careful in:

- `Advanced Tweaks`
- `App Debloater`
- `Service Manager`
- `Registry Manager`
- `Network Optimizer`

## Restore Points

Higher-impact operations can request a restore point before running. This is especially important for:

- advanced system tweaks
- app removal
- registry changes
- broad privacy or network changes
- AI-assisted automatic fix application

If a restore point is offered, it is usually a good idea to accept it.


### Requirements

- Windows 10 or Windows 11
- Administrator access for most features
- .NET 8 SDK for local builds

## Troubleshooting

If something does not behave as expected:

1. Make sure SynTweaks is running as Administrator.
2. Check the newest log file in `%APPDATA%\SynTweaks\logs\`.
3. Reboot if the tool reports that a restart, sign-out, or Explorer restart is required.
4. Re-test after one change at a time instead of stacking many aggressive actions together.
5. Use `Report Center` to preview diagnostics or send a report.

Common reasons for failure:

- Windows permissions or elevation issues
- security software blocking PowerShell or system commands
- network restrictions affecting AI or reporting
- Windows components already being damaged before the action runs
- applying multiple aggressive tweaks without validating each change

## Access, Support, and Redistribution

Because this is a private project:

- there is no public contribution workflow
- there is no redistribution permission by default
- there is no open-source license grant
- support should go through direct contact, approved testers, or the in-app report system

## Credits

- Product: `SynTweaks`
- Version: `2.0.0`
- Developer: `SyntaX`
- Platform: `Windows 10 / 11`
- Runtime: `C# / .NET 8`
