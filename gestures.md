---
title: Gestures
description: Gesture and navigation reference for Dextera Launcher.
permalink: /gestures/
---

## Primary gestures

| Gesture | Action |
|---------|--------|
| **Flick search bar** left / right | Jump one adjacent page |
| **Hold + drag** on search bar | Page **scrubber** (dots under thumb); large page name popup |
| **Tap gear** on search bar | Open **page overview** |
| **Drag A–Z sidebar** | Jump app list to letter / pin / frequently used |
| **Drag Contacts rail** | Jump the contacts list (when enabled) |
| **Long-press app / contact row** | Anchored context menu |
| **Pinch in** or **long-press empty home** | Page overview (rearrange workspace) |
| **System back** | Close menus, clear search; page cycle only when **not** in traditional swiping mode |
| **Long-hold back** (optional) | Run the configured gesture action (page jump, first page, left-handed toggle, …) |
| **Pull down** (reachability) | Slightly lowers workspace for one-handed use |
| **Double-tap header** (optional) | Configured action (page, first page, left-handed, …) |
| **Home button / home gesture** | Return to Dextera; see [Home action](#home-action) |
| **Horizontal swipe** (traditional swiping mode) | Classic free-swipe between pages |

## Home action {#home-action}

In **Settings → Touch & Gestures → Home button & gesture** you can assign an action. Special case for **First page**:

1. **While in another app** — Home returns you to the **page you left** (continuity).  
2. **Home again while already on Dextera** — jumps to the **first page**.  

Default (no custom action) still uses continuity when returning from an app and reset-to-first when already home.

## Page scrubber

<p align="center">
  <img class="shot" src="{{ '/assets/images/05_page_scrubber.png' | relative_url }}" alt="Page scrubber" width="320" />
</p>

- Quick swipe = one page  
- Sustained drag = continuous scrub with haptic feedback  
- Scrub UI always clears on finger up (safety timeout so blur/dim cannot stick)  

## Search keyboard & back

- Back closes context menus first (while open), then clears focus/query and restores home  
- IME padding keeps results above the keyboard  
- Native back-handler integration respects system swipe-to-go-back  

## Configure gestures

Open **Settings → Touch & Gestures** (or **Page settings** from overview for page-specific options):

- Home screen gestures master switch  
- **Home button & gesture** action (including **First page**)  
- Double-tap header action  
- Long-hold back + action  
- Traditional swiping mode  

## Tips

1. Keep your thumb on the search bar for multi-page navigation without reaching the top of the screen.  
2. Use **page overview** (pinch, empty long-press, or the search **gear**) to reorder pages and open **Page settings**.  
3. Prefer **First page** Home action if you want “back to where I was” once, then a second Home to land on the first page.  
