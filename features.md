---
title: Features
description: Complete feature guide for Dextera Launcher — search, notifications, media, security, and more.
permalink: /features/
---

Dextera is a modern Android home launcher built with **Kotlin** and **Jetpack Compose**. It replaces the stock home screen with a gesture-first workspace: unified search, multi-page panels, smart notifications, media controls, security, and deep appearance customization.

> **Status:** Public beta (`0.4.0-beta`). Feature set for this cycle is complete; updates emphasize polish, stability, and Play compliance.

## Smart notification center

A custom notification tray that reimagines how notifications appear on the home screen.

- **Intelligent card stacking** — same-app notifications group into layered cards that expand on tap  
- **Pin apps to the top** — long-press a card’s app icon to keep that app’s notifications sorted above others  
- **Lock pinned notifications** (Page settings → Notifications) — when on, notifications from pinned apps **cannot be swiped away or bulk-cleared** until you unpin the app or turn the lock off  
- **Robust intent handling** — works with Android 12+ background activity restrictions  
- **System filtering** — reduces noisy persistent/system service clutter  
- **Inline actions** — quick reply, mark read, dismiss where the system allows  
- **Badges** on app list icons  
- Fullscreen compact **icon strip** under the cutout when the status bar is hidden  
- Optional pin-to **Scratch Board** (swipe right on a card when Scratch Board is enabled)

Requires **Notification listener** access for Dextera.

## Interactive media hub

A layout-aware media experience integrated into the workspace.

- Dedicated **Music** page when a session is active  
- Physics-based play/pause gestures (e.g. swipe on artwork with spring feedback)  
- Floating transport controls and marquee metadata  
- Smart volume routing to local `STREAM_MUSIC` or active cast sessions  
- Optional **button-style** transport controls in Music page settings  

## Unified search engine

Tap the floating **Search** bar for on-device + web search.

<p align="center">
  <img class="shot" src="{{ '/assets/images/06_search.png' | relative_url }}" alt="Unified search" width="320" />
</p>

| Type | Notes |
|------|--------|
| **Apps** | Launch; long-press for context menu (isolated from the home list under the overlay) |
| **Contacts** | Call / message; long-press for contact menu |
| **Settings** | Jump into launcher settings categories |
| **Files** | Local files from **folders you add** (system folder picker / SAF) |
| **Web** | Suggestions + open in browser (engine selectable) |

Category chips: **All · Contacts · Apps · Web · Settings**. Optional **search history** when the query is empty (recent apps grid + recent non-app hits). Empty search can show recent apps; labels sit above the search chrome so they aren’t clipped.

### Search bar gear

The **gear** on the search bar opens **page overview** (same workspace as pinch / long-press empty home) — not the full Settings app. Full Settings and per-page settings live under overview and the in-app Settings panel.

Typing does not reshape the home drawer under the overlay; home stays mounted and faded while search is open.

## Modern app drawer

- Alphabetical list with optional **pinned** and **Frequently used** sections  
- Fast A–Z sidebar (or dots mode) with large letter popup; scalable letter size and optional idle fade  
- **Contacts** page can use its own quick-scroll rail (or sync style with the app list)  
- Category chips / folders (Social, Utilities, Media, …)  
- Notification badges  
- Launch respects **app lock** and wellbeing options when enabled  

## App & contact context menus

Long-press for an **anchored pointer menu** (not a full-screen sheet). Menus are **source-scoped** so search results and the homescreen don’t steal each other’s anchors or leave menus stranded after focus changes.

| Action | Purpose |
|--------|---------|
| **Info** | System app details |
| **Pin / Unpin** | Keep at top of app list |
| **Lock / Unlock** | Biometric gate (needs Global app locker) |
| **Hide / Show** | Remove from list (Wellbeing) |
| **Folder** | Add to category groups |
| **Uninstall** | System uninstall flow |

Contacts: Call, Message, Pin, Delete (with contacts permission).

## Weather & clock

**Clock styles:** Dextera Date, Minimal Digital, Bold Accent, Classic Analog (extras may require Pro).

Options include glass clock background, invert text, 24-hour time, °F / °C, live weather with forecast overlay, and optional **manual ZIP** location (Pro).

With **Hide status bar**, optional **network speed** ↑/↓ can show next to the time.

## Security

### Uninstallation protection

Registers Dextera as a **device admin** so casual uninstall is blocked until admin is deactivated in system settings.

### Global app locker

Accessibility service **Dextera App Locker** intercepts locked apps (including from Recents) and requires biometric / device credential. Opaque cover so content is not readable under the prompt. Independent of device admin.

**Why Accessibility?** Android has no dedicated public API for reliable app-open intercept. The service is used only for this security feature — not as an accessibility tool for disabilities, and not to read passwords or send data off-device. See [Why Dextera uses Accessibility]({{ '/permissions/#accessibility' | relative_url }}).

### Verification codes / OTP (optional)

Extract one-time codes from **messaging-app notifications** (notification access) and show a home OTP chip (copy / floating popup when overlay permission allows). Does not use SMS inbox or `READ_SMS`.

## Wallpaper & contrast

- **System wallpaper** (live pass-through when the OEM allows), **Pitch Black**, **Bing Daily** (Pro), built-in catalog  
- **Local images** — pick photos via the **system photo picker** (no broad photo-library permission). Up to **7** photos stay in a library; tap to use, long-press to remove  
- **Dynamic (day / night)** — import **GNOME** timed packs (or use the preinstalled **Horizon** pack); frames follow the clock with crossfades  
- **Per-page wallpapers** — turn off “sync wallpaper” in **Page overview**, then set a wallpaper for the centered page only  
- Text colors adapt to wallpaper luminance; optional **blur** (Pro) and **dim**  

## Widgets & custom pages

- Free-form **widget canvas** with snap grid, resize, live preview, and per-page grid size presets  
- Dextera’s **own widget picker** with previews  
- **Traditional swiping** mode (optional) for classic page swipes; landscape tablets keep a usable docked workspace  
- Custom page **rename** and orphaned-widget cleanup  

## Scratch Board

Notes, clipboard captures, and pinned notifications in a dedicated page / overlay. Share-to-Scratch-Board is supported for files. Optional S Pen detach jump (Samsung) when Scratch Board is enabled.

## Related pages

- [Gestures & navigation]({{ '/gestures/' | relative_url }})  
- [Launcher pages]({{ '/pages/' | relative_url }})  
- [Settings]({{ '/settings/' | relative_url }})  
- [Permissions]({{ '/permissions/' | relative_url }})  
