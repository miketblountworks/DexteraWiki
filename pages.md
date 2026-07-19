---
title: Launcher pages
description: App list, contacts, recents, music, notifications, quick settings, widgets, and Scratch Board.
permalink: /pages/
---

Default pages (order configurable in **Settings → Launcher Pages**):

| Page | Role |
|------|------|
| **App List** | Main drawer + sidebar |
| **Contacts** | Device + launcher contacts; call/message; pin; optional quick-scroll rail |
| **Recents** | Recent apps; swipe to close; long-press for menu |
| **Music** | Now playing / media hub |
| **Notifications** | Custom notification center |
| **Scratch Board** | Notes, clipboard, pinned notifications |
| **Quick Settings** | Fast toggles / system-adjacent controls (Pro for adding) |
| **Custom / Widgets** | Free-form widget canvas pages (Pro for extras) |

<p align="center">
  <img class="shot" src="{{ '/assets/images/03_page.png' | relative_url }}" alt="Launcher page example" width="320" />
</p>

## Page overview

<p align="center">
  <img class="shot" src="{{ '/assets/images/07_page_overview.png' | relative_url }}" alt="Page overview" width="320" />
</p>

Open overview by:

- Pinch in or long-press empty home  
- Tapping the **gear** on the floating search bar  

From overview you can reorder pages, open **Page settings** for the centered card, toggle **sync wallpaper**, set **page wallpaper**, and manage widget pages (grid size presets, add widgets).

**Back from Page settings** returns you to page overview (not straight to the home screen).

## Dynamic visibility

Some pages hide when empty (for example no media session or no visible notifications), then reappear when content returns.

## App list details

- Alphabetical launchable apps  
- Optional **pinned** apps at top  
- Optional **Frequently used** (usage stats + limit)  
- Category chips when folders have apps  
- Notification badges  
- Launch respects app lock and usage breaker if enabled  

### Sidebar (quick scroll)

- Letters **A–Z** (or **dots** mode)  
- Markers for pinned and frequently used  
- Large letter/icon popup while scrubbing  
- Letter size levels and optional idle fade  

### Folders / categories

Apps can be added to groups (Social, Utilities, Media, …) from the context menu **Folder** face. Home category row filters the list by group.

## Contacts page

- Merged system + launcher contacts  
- Swipe for message shortcuts; long-press for contact menu  
- Optional **quick-scroll rail** (can sync styling with the app list or use its own dots / fade / letter size)

## Notifications page

Requires notification listener access.

- Grouped stacks by app  
- Expand, dismiss, inline actions, quick reply  
- **Pin apps** to the top of the list (long-press app icon on a card)  
- **Lock pinned notifications** (Page settings) — blocks swipe-dismiss and **Clear All** for those apps  
- Category filters (Wellbeing / notification settings)  
- Safe deep-link / pending-intent handling for modern Android  

## Media page

When a media session is active:

- Play/pause gestures with spring feedback  
- Transport controls and marquee metadata  
- Volume routing to local stream or cast session  

## Quick Settings

<p align="center">
  <img class="shot" src="{{ '/assets/images/04_quick_settings.png' | relative_url }}" alt="Quick Settings page" width="320" />
</p>

Fast system-adjacent toggles living as a first-class launcher page rather than only a status-bar shade. The panel scrolls if content is tall.

## Widgets

- Free-form canvas with snap grid and cell overlay while editing  
- Resize, drag, landing highlight, auto-edit on add  
- Per-page **grid size presets** (including dense layouts)  
- Dextera widget picker with previews  
- Custom page **rename** and cleanup of orphaned widgets  

## Scratch Board

Timeline of notes, clipboard captures, and notifications you pin. Optional share-into-Scratch-Board for files. Can open as a page or overlay.
