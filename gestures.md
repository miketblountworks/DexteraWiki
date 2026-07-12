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
| **Drag A–Z sidebar** | Jump app list to letter / pin / frequently used |
| **Long-press app / contact row** | Anchored context menu |
| **Pinch in** or **long-press empty home** | Page overview (rearrange workspace) |
| **System back** | Close menus, clear search, page cycle (configurable) |
| **Long-hold back** (optional) | Jump to a configured page |
| **Pull down** (reachability) | Slightly lowers workspace for one-handed use |
| **Double-tap** (optional) | Sleep / gesture action when enabled in Settings |

## Page scrubber

<p align="center">
  <img class="shot" src="{{ '/assets/images/05_page_scrubber.png' | relative_url }}" alt="Page scrubber" width="320" />
</p>

- Quick swipe = one page  
- Sustained drag = continuous scrub with haptic feedback  
- Scrub UI always clears on finger up (safety timeout so blur/dim cannot stick)  

## Search keyboard & back

- Back clears focus/query and restores home  
- IME padding keeps results above the keyboard  
- Native back-handler integration respects system swipe-to-go-back  

## Configure gestures

Open **Settings → Touch & Gestures**:

- Home screen gestures master switch  
- Long-hold back + target page  
- Documented actions for swipe down, double tap, pinch, hold back  

## Tips

1. Keep your thumb on the search bar for multi-page navigation without reaching the top of the screen.  
2. Use page overview (pinch) when reordering pages or managing widgets.  
3. If the screen ever looks “stuck” blurred after scrubbing, update to a build that includes scrub gesture cleanup — blur should clear with the finger.  
