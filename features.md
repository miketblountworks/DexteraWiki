---
title: Features
description: Complete feature guide for Dextera Launcher — search, notifications, media, security, and more.
permalink: /features/
---

Dextera is a modern Android home launcher built with **Kotlin** and **Jetpack Compose**. It replaces the stock home screen with a gesture-first workspace: unified search, multi-page panels, smart notifications, media controls, security, and deep appearance customization.

> **Status:** Active development. Features and UI continue to evolve.

## Smart notification center

A custom notification tray that reimagines how notifications appear on the home screen.

- **Intelligent card stacking** — same-app notifications group into layered cards that expand on tap  
- **Robust intent handling** — works with Android 12+ background activity restrictions via `ActivityOptions` fallbacks  
- **System filtering** — reduces noisy persistent/system service clutter  
- **Inline actions** — quick reply, mark read, dismiss where the system allows  
- **Badges** on app list icons  
- Fullscreen compact **icon strip** under the cutout when the status bar is hidden  

Requires **Notification listener** access for Dextera.

## Interactive media hub

A layout-aware media experience integrated into the workspace.

- Dedicated **Music** page when a session is active  
- Physics-based play/pause gestures (e.g. swipe on artwork with spring feedback)  
- Floating transport controls and marquee metadata  
- Smart volume routing to local `STREAM_MUSIC` or active cast sessions  

## Unified search engine

Tap the floating **Search** bar for on-device + web search.

<p align="center">
  <img class="shot" src="{{ '/assets/images/06_search.png' | relative_url }}" alt="Unified search" width="320" />
</p>

| Type | Notes |
|------|--------|
| **Apps** | Launch; long-press for menu |
| **Contacts** | Call / message |
| **Settings** | Jump into launcher or system areas |
| **Files** | Local files (media permission / indexed folders) |
| **SMS** | Optional SMS search |
| **Web** | Suggestions + open in browser (engine selectable) |

Category chips: **All · Contacts · Apps · Web · Settings**. Optional search history when the query is empty. Typing does not mutate the drawer under the overlay.

## Modern app drawer

- Alphabetical list with optional **pinned** and **Frequently used** sections  
- Fast A–Z sidebar (or dots mode) with large letter popup  
- Category chips / folders (Social, Utilities, Media, …)  
- Notification badges  
- Launch respects **app lock** and wellbeing options when enabled  

## App & contact context menus

Long-press for an **anchored pointer menu** (not a full-screen sheet).

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

**Clock styles:** Dextera Date, Minimal Digital, Bold Accent, Classic Analog.

Options include glass clock background, invert text, 24-hour time, °F / °C, and live weather with forecast overlay (location optional).

With **Hide status bar**, optional **network speed** ↑/↓ can show next to the time.

## Security

### Uninstallation protection

Registers Dextera as a **device admin** so casual uninstall is blocked until admin is deactivated in system settings.

### Global app locker

Accessibility service **Dextera App Locker** intercepts locked apps (including from Recents) and requires biometric / device credential. Opaque cover so content is not readable under the prompt. Independent of device admin.

### SMS OTP (optional)

Extract verification codes from SMS/notifications and show a home OTP chip (copy / floating popup when overlay permission allows).

## Wallpaper & contrast

- **Pitch Black**, **Bing Daily**, or built-in catalog images  
- Text colors adapt to wallpaper luminance  
- Optional blur and dim  

## Related pages

- [Gestures & navigation]({{ '/gestures/' | relative_url }})  
- [Launcher pages]({{ '/pages/' | relative_url }})  
- [Settings]({{ '/settings/' | relative_url }})  
- [Permissions]({{ '/permissions/' | relative_url }})  
