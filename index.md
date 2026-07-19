---
title: Home
hero: true
hero_title: A modern Android home, documented.
hero_subtitle: Dextera is a highly customizable launcher built with Kotlin and Jetpack Compose — smart notifications, unified search, media controls, and a gesture-first workspace.
hero_ctas: true
description: Official wiki and documentation for Dextera Launcher.
---

<p><span class="status-pill">● Public beta · 0.4.0-beta</span></p>

Dextera replaces the stock Android home screen with a fluid, premium experience. Built by **Dextera Labs**, this wiki is the public user documentation for Dextera Launcher. The app is **proprietary software** — not open source.

## Highlights

<div class="card-grid">
  <div class="card">
    <h3>Smart notifications</h3>
    <p>App-grouped card stacks, pin-to-top apps, optional lock so pinned apps can’t be swiped away, and inline actions.</p>
  </div>
  <div class="card">
    <h3>Unified search</h3>
    <p>Apps, contacts, settings, local files (folders you add), and web suggestions from one floating search bar.</p>
  </div>
  <div class="card">
    <h3>Multi-page workspace</h3>
    <p>Apps, contacts, recents, music, notifications, widgets, Scratch Board — scrub or swipe between pages with your thumb.</p>
  </div>
  <div class="card">
    <h3>Privacy-first design</h3>
    <p>Most processing stays on-device. Photo picker for wallpapers; file search via folders you choose — no broad photo library permission.</p>
  </div>
</div>

## Screenshots

<div class="shot-grid">
  <figure class="shot-card">
    <img src="{{ '/assets/images/01_home.png' | relative_url }}" alt="Dextera home screen" />
    <figcaption>Home workspace with clock, weather, and app list</figcaption>
  </figure>
  <figure class="shot-card">
    <img src="{{ '/assets/images/06_search.png' | relative_url }}" alt="Unified search" />
    <figcaption>Unified search overlay</figcaption>
  </figure>
  <figure class="shot-card">
    <img src="{{ '/assets/images/07_page_overview.png' | relative_url }}" alt="Page overview" />
    <figcaption>Page overview — also opened from the search bar gear</figcaption>
  </figure>
  <figure class="shot-card">
    <img src="{{ '/assets/images/02_settings.png' | relative_url }}" alt="Settings entry" />
    <figcaption>Settings from page overview (Page settings) or the full Settings entry</figcaption>
  </figure>
</div>

## Wiki map

| Page | What you’ll find |
|------|------------------|
| [Getting started]({{ '/getting-started/' | relative_url }}) | Onboarding, default home, first-run tips |
| [Features]({{ '/features/' | relative_url }}) | Full feature guide with UI details |
| [Gestures]({{ '/gestures/' | relative_url }}) | Navigation, scrubber, Home action, reachability |
| [Pages]({{ '/pages/' | relative_url }}) | App list, contacts, media, notifications, widgets |
| [Settings]({{ '/settings/' | relative_url }}) | Appearance, wallpapers, wellbeing, security, search |
| [Permissions]({{ '/permissions/' | relative_url }}) | What each permission is for |
| [Privacy]({{ '/privacy/' | relative_url }}) | Full privacy policy |

## Tech stack

- **Language:** Kotlin  
- **UI:** Jetpack Compose  
- **Integrations:** `NotificationListenerService`, `MediaController`, `AudioManager`, accessibility app locker, device admin  

## Status

**Public beta (`0.4.0-beta`).** The core launcher loop is feature-complete for this cycle. Updates emphasize stability, polish, and Play compliance rather than large new surface area. Prefer this wiki for user-facing docs and policy text.

**Developer:** Dextera Labs  
**License:** Proprietary — not open source. This wiki is public documentation only.
