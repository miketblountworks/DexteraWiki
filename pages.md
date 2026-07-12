---
title: Launcher pages
description: App list, contacts, recents, music, notifications, quick settings, and widgets.
permalink: /pages/
---

Default pages (order configurable in **Settings → Launcher Pages**):

| Page | Role |
|------|------|
| **App List** | Main drawer + sidebar |
| **Contacts** | Device + launcher contacts; call/message; pin |
| **Recents** | Recent apps; swipe to close; long-press for menu |
| **Music** | Now playing / media hub |
| **Notifications** | Custom notification center |
| **Quick Settings** | Fast toggles / system-adjacent controls |
| **Widgets** | Widget host pages |

<p align="center">
  <img class="shot" src="{{ '/assets/images/03_page.png' | relative_url }}" alt="Launcher page example" width="320" />
</p>

## Page overview

<p align="center">
  <img class="shot" src="{{ '/assets/images/07_page_overview.png' | relative_url }}" alt="Page overview" width="320" />
</p>

Pinch or long-press empty space to open overview, reorder/manage pages, and work with widgets.

## Dynamic visibility

Some pages hide when empty (for example no media session or no visible notifications), then reappear when content returns.

## App list details

- Alphabetical launchable apps  
- Optional **pinned** apps at top  
- Optional **Frequently used** (usage stats + limit 4 / 6 / 8)  
- Category chips when folders have apps  
- Notification badges  
- Launch respects app lock and usage breaker if enabled  

### Sidebar (quick scroll)

- Letters **A–Z** (or **dots** mode)  
- Markers for pinned and frequently used  
- Large letter/icon popup while scrubbing  
- Optional idle fade  

### Folders / categories

Apps can be added to groups (Social, Utilities, Media, …) from the context menu **Folder** face. Home category row filters the list by group.

## Notifications page

Requires notification listener access.

- Grouped stacks by app  
- Expand, dismiss, inline actions, quick reply  
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

Fast system-adjacent toggles living as a first-class launcher page rather than only a status-bar shade.

## Widgets

Add, remove, and resize widgets via overview and the widget host APIs on dedicated widget pages.
