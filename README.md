# MemoryCleaner

**A lightweight, free Windows memory cleaner that frees memory with one click and cleans automatically under the conditions you set.**

English · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · [Español](README.es.md) · [Português (Brasil)](README.pt-BR.md) · [Français](README.fr.md)

> This document is a translation. If anything differs, the [Korean version](README.ko.md) is authoritative.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20(64--bit)-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
![Version](https://img.shields.io/badge/version-3.0.0-blue)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/memorycleaner?lang=en)

![MemoryCleaner window](images/memorycleaner-en.webp)

## Overview

MemoryCleaner shows how much memory is in use right now, and one click on **Clean memory** takes back the cache Windows is holding on to and the memory running programs aren't using at the moment.

You can set it to clean on its own when memory usage gets high, at a fixed interval, or when cache builds up and free memory runs low. While a game or video is running full screen, it skips cleaning so it never gets in the way.

Closing the window sends it to the notification area (system tray), where it keeps working quietly. After the window closes, MemoryCleaner lets go of everything the window used, so while waiting in the tray it uses only about 1 MB itself.

## Features

- **One-click cleaning** — Clean memory with the **Clean memory** button or a single click on the tray icon.
- **Choose what to clean** — Pick the areas to clean yourself: file cache, working set, standby list, registry cache, combine memory and more.
- **Automatic cleaning** — Cleans when physical memory · virtual memory · working set usage goes over a threshold, or at a fixed interval.
- **Anti-stutter for games** — When cache (the standby list) builds up and free memory runs low, it purges just the cache.
- **Full-screen detection** — Skips automatic cleaning while a game, video or presentation is running full screen.
- **Memory status** — See physical memory, virtual memory, working set and cached memory on the main screen and the tray icon.
- **Lightweight** — A single executable that uses only about 1 MB while waiting in the tray.
- **9 languages** — Korean · English · Japanese · Chinese · Russian · Italian · French · Spanish · Arabic.

## Download / Installation

| Type | Link |
|---|---|
| Installer | [Download](https://down.kilho.net/memorycleaner?lang=en) |
| Portable (ZIP) | [Download](https://down.kilho.net/memorycleaner?lang=en&nosetup) |

The installer launches MemoryCleaner as soon as setup finishes and turns on **Run on system start**, so it starts in the tray every time you sign in to Windows. For the portable version, unzip it and run `MemoryCleaner.exe`. Both versions have the same features.

Cleaning memory requires administrator rights, so Windows shows an administrator permission prompt when you run it. Click **Yes**.

## Usage

### Getting started

1. Run MemoryCleaner and click **Yes** in the administrator permission prompt.
2. **Home** shows physical memory usage as a bar and numbers, with virtual memory · working set · cached memory below it. The values refresh every second.
3. Click **Clean memory**; the button changes to **Cleaning**, and when it's done you can see the lower usage right away.
4. To have it clean on its own, click **Config** and turn on the conditions you want under **Auto clean**.
5. Closing the window keeps MemoryCleaner running in the tray. Click the tray icon to open the window again.

### Screen layout

**Top buttons**

| Element | What it does |
|---|---|
| **Home** | The main screen with the memory status and the **Clean memory** button |
| **Config** | Auto clean · Clean targets · General |
| **Donate** | Opens the donation page |
| KILHO.net logo | Opens the MemoryCleaner product page |

**Home**

| Element | What it shows |
|---|---|
| Bar | Physical memory usage |
| **Physical** | Used / total (MB) and usage |
| **Virtual** | Virtual memory usage including the page file |
| **working set** | Memory held by running programs, and its share |
| **Cached** | Memory Windows keeps as cache (the same value as "Cached" in Task Manager) and its share of physical memory |
| **Clean memory** | Cleans right now. Changes to **Cleaning** while it works |

**Config**

| Group | Items |
|---|---|
| **Auto clean** | **Clean when physical memory usage is higher than (%)** · **Clean when pagefile usage is higher than (%)** · **Clean when total workingset usage is higher than (%)** · **Clean automatically if interval (minutes) exceeded.** · **Purge cached (standby list) memory (anti-stutter)** · **Skip cleaning in full screen** |
| **Clean targets** | **File cache** · **working set** · **Standby list (low priority)** · **Registry cache** · **Combine memory** · **Standby list \*** · **Modified page list \*** |
| **General** | **Run on system start** · **Clean when you click on the task icon** |
| Bottom | Current version and the **Defaults** button |

**Tray icon**

| Action | Result |
|---|---|
| Hover | Physical memory · virtual memory · working set usage |
| Left-click | Opens the window (cleans right away if **Clean when you click on the task icon** is on) |
| Right-click | **MemoryCleaner** (open window) · **Crafted by Kilho** (product page) · **Quit** |

While cleaning, the tray icon changes shape, so you can tell it's working without opening the window.

**Clean targets** — what each one frees

| Item | What it frees | Default |
|---|---|---|
| **File cache** | Cache Windows builds up while reading and writing files | On |
| **working set** | Memory running programs aren't using at the moment | On |
| **Standby list (low priority)** | The part of the cache least likely to be used again | On |
| **Registry cache** | Cache built up while reading the registry | On |
| **Combine memory** | Merges identical memory contents into one to free space | On |
| **Standby list \*** | The entire cache | Off |
| **Modified page list \*** | Memory waiting to be written to disk | Off |

Items marked `*` can cause brief stutters during games or video playback, so they start off.

### When you want to…

**Clean memory right now**
Click **Clean memory** on **Home**. The button changes to **Cleaning** while it works and back to **Clean memory** when it's done. Click it once when your PC feels sluggish after running many programs for a long time, or right before launching a big game or editing program.

**Clean from the tray icon without opening the window**
Turn on **Config → Clean when you click on the task icon**, and a single click on the tray icon cleans memory. When it's done, an "Optimized memory." notification appears. While this is on, open the window with a right-click on the tray icon → **MemoryCleaner**.

**Check memory status without the window**
Hover over the tray icon to see physical memory · virtual memory · working set usage — enough to judge whether cleaning is needed without opening the window.

**Clean automatically when memory runs short**
Under **Config → Auto clean**, turn on **Clean when physical memory usage is higher than (%)** and choose a threshold (30 – 90%) in the box next to it. When usage goes over the threshold, MemoryCleaner cleans on its own. If you rely heavily on the page file, also turn on **Clean when pagefile usage is higher than (%)**; if programs hogging memory is the problem, turn on **Clean when total workingset usage is higher than (%)**. When cleaning doesn't bring usage down, it waits before cleaning again rather than cleaning over and over, so cleaning never becomes a burden itself.

**Clean at a regular interval**
Turn on **Clean automatically if interval (minutes) exceeded.** and pick 5 · 10 · 20 · 30 · 40 · 50 · 60 minutes; it then cleans at that interval regardless of usage. Good for keeping a PC that stays on for long periods light.

**When a game gets choppier the longer you play (cache purging)**
Sometimes a game stutters more and more the longer it runs, until only restarting the game fixes it. That's because Windows keeps files it has read as cache (the standby list); when this builds up and free memory runs out, Windows has to reclaim that cache in a hurry, which makes the game stutter for a moment. Turn on **Purge cached (standby list) memory (anti-stutter)**, and when the cache goes over the **Purge when cached (MB) is higher than** threshold (512 · 1024 · 2048 · 4096 MB) while free memory drops below the **Purge when free memory (MB) is lower than** threshold (1024 · 2048 · 4096 · 8192 · 16384 MB), it purges just the cache ahead of time. It acts only when both conditions are met, and after purging the conditions clear by themselves, so it only steps in when needed.

Setting the free-memory threshold to half the memory installed in your PC works well.

| Installed memory | Purge when free memory (MB) is lower than |
|---|---|
| 8 GB | 4096 (default) |
| 16 GB | 8192 |
| 32 GB | 16384 |

You don't need to turn it on only while gaming. It uses only about 1 MB in the tray and acts only when the conditions are met, so just leave it on.

**Leave games and movies alone**
**Skip cleaning in full screen** is on from the start. While a game, video or presentation runs full screen, automatic cleaning is skipped so the screen never stutters. Once you leave full screen, it works as usual again.

**Choose what to clean yourself**
Check the areas to clean under **Config → Clean targets**. Both the **Clean memory** button and automatic cleaning follow these items. If nothing is checked there's nothing to do, so the **Clean memory** button is grayed out.

**When you want stronger cleaning**
Turning on **Standby list \*** and **Modified page list \*** also frees the entire cache and the memory waiting to be written, which frees the most memory. They can cause brief stutters during games or video playback, though, so turn them on only when needed and keep them off otherwise.

**Wondering what "Cached" means**
**Cached** on **Home** is memory Windows keeps in case it's needed again — the same value as "Cached" in Task Manager. A large value isn't bad in itself, but if games stutter, try the cache purging above.

**Start automatically with Windows**
Turn on **Config → Run on system start**, and MemoryCleaner starts quietly in the tray shortly after you sign in to Windows — without an administrator permission prompt. It's on from the start in the installed version.

**Keep it running after closing the window**
Clicking the window's X doesn't quit MemoryCleaner; it goes to the tray and keeps cleaning automatically. It also lets go of all the memory the window used, so leaving it running costs almost nothing. To quit completely, right-click the tray icon → **Quit** and confirm.

**Quitting while cleaning**
If you quit while cleaning is in progress, the button changes to **Exit after cleaning**, and the program ends once cleaning is finished. Cleaning is never cut off halfway.

**Reset all settings**
Click **Defaults** at the bottom of **Config** and confirm to return all auto clean and clean target settings to their defaults. **Run on system start** is left as it is.

**Running it again while it's already running**
Only one MemoryCleaner runs at a time. Running it again while it's in the tray doesn't start a new copy; it opens the window of the one already running.

## Configuration

Every setting is saved as soon as you change it and used again at the next launch.

| Item | Default |
|---|---|
| Cleaning by physical memory · pagefile · working set usage | Off (90% when turned on) |
| Clean automatically if interval (minutes) exceeded. | Off (30 minutes when turned on) |
| Purge cached (standby list) memory | Off (cached ≥ 1024 MB · free < 4096 MB when turned on) |
| Skip cleaning in full screen | On |
| Clean targets | File cache · working set · Standby list (low priority) · Registry cache · Combine memory |
| Run on system start | On in the installed version |
| Clean when you click on the task icon | Off |
| Language | Follows the Windows region setting (English if the language isn't supported) |

## Requirements

- Windows 10 · Windows 11 (64-bit)
- Administrator rights — needed to clean memory. A permission prompt appears when you run it (but not when it starts through **Run on system start**).
- No other components to install.
- The internet connection is used only for new-version notices.

## Updates

MemoryCleaner does **not** update itself. At startup it checks for a new version and shows a notice; clicking **[Yes]** opens the download page and closes the program. New versions are released manually after internal testing and announced on the [MemoryCleaner page](https://kilho.net/memorycleaner). See the [update policy notice](https://en.kilho.net/archives/notice/2940).

**Version history**

| Version | Date | Changes |
|---|---|---|
| 3.0.0 | 2026-09-29 | Rebuilt in pure C, faster and more stable — tray memory use down by more than 95% and program size down by about 98%, choose what to clean, automatic cache purging (anti-stutter for games), cached memory shown on the main screen, default cleanup settings tuned for games and video, button to restore defaults, more reliable update checks and startup |
| 2.0.3 | 2026-09-03 | Better full-screen detection so games and videos aren't interrupted, more stable shutdown, more accurate completion notifications, optimized repeated cleaning, more stable settings |
| 2.0.2 | 2026-08-13 | Option to skip cleaning while in full screen, auto-start settings removed on uninstall, more reliable settings loading and auto-start |
| 2.0.1 | 2026-07-13 | Stronger browser memory cleanup, better long-running stability, more reliable notifications and settings, Spanish added |

## License

MemoryCleaner is **freeware**. Use it for free without restriction anywhere — at work, at home, in government offices or at school — and redistribute it freely.

## Links

- Website: <https://kilho.net/memorycleaner>
- Forum: <https://kilho.top/forum/qna>
- X (Twitter): <https://www.twitter.com/kilhonet>

© KILHO.NET
