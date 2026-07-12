---
title: Home
hero: true
hero_title: A modern Android home, documented.
hero_subtitle: Dextera is a highly customizable launcher built with Kotlin and Jetpack Compose — smart notifications, unified search, media controls, and a gesture-first workspace.
hero_ctas: true
description: Official wiki and documentation for Dextera Launcher.
---

<p><span class="status-pill">● Active development</span></p>

Dextera replaces the stock Android home screen with a fluid, premium experience. Built by **Dextera Labs**, this wiki is the public user documentation for Dextera Launcher. The app is **proprietary software** — not open source.

## Highlights

<div class="card-grid">
  <div class="card">
    <h3>Smart notifications</h3>
    <p>App-grouped card stacks, inline actions, and badges — without the usual tray clutter.</p>
  </div>
  <div class="card">
    <h3>Unified search</h3>
    <p>Apps, contacts, settings, files, and web suggestions from one floating search bar.</p>
  </div>
  <div class="card">
    <h3>Multi-page workspace</h3>
    <p>Apps, contacts, recents, music, notifications, quick settings, and widgets — scrub between pages with your thumb.</p>
  </div>
  <div class="card">
    <h3>Privacy-first design</h3>
    <p>Most processing stays on-device. No Dextera account. No ads SDK in the core design.</p>
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
    <figcaption>Page overview for rearranging the workspace</figcaption>
  </figure>
  <figure class="shot-card">
    <img src="{{ '/assets/images/02_settings.png' | relative_url }}" alt="Settings entry point" />
    <figcaption>Settings via the gear on the search bar</figcaption>
  </figure>
</div>

## Wiki map

| Page | What you’ll find |
|------|------------------|
| [Getting started]({{ '/getting-started/' | relative_url }}) | Onboarding, default home, first-run tips |
| [Features]({{ '/features/' | relative_url }}) | Full feature guide with UI details |
| [Gestures]({{ '/gestures/' | relative_url }}) | Navigation, scrubber, reachability |
| [Pages]({{ '/pages/' | relative_url }}) | App list, contacts, media, notifications, widgets |
| [Settings]({{ '/settings/' | relative_url }}) | Appearance, wellbeing, security, search |
| [Permissions]({{ '/permissions/' | relative_url }}) | What each permission is for |
| [Privacy]({{ '/privacy/' | relative_url }}) | Full privacy policy |

## Tech stack

- **Language:** Kotlin  
- **UI:** Jetpack Compose  
- **Integrations:** `NotificationListenerService`, `MediaController`, `AudioManager`, accessibility app locker, device admin  

## Status

Dextera is under active development. Core features, UI, and system architecture continue to iterate. Prefer this wiki for user-facing docs and policy text.

**Developer:** Dextera Labs  
**License:** Proprietary — not open source. This wiki is public documentation only.
