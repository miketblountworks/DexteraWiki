---
title: Permissions
description: Why Dextera asks for each Android permission or system access.
permalink: /permissions/
---

Dextera only uses permissions needed for features you enable. Optional items can be deferred and enabled later in Settings or system Settings.

## Reference

| Permission / access | Used for |
|---------------------|----------|
| **Default home role** | Home button opens Dextera |
| **Notification listener** | Notification center, badges, media, OTP fallbacks |
| **Contacts** (read/write) | Contact page, search, delete |
| **Location (approx.)** | Weather |
| **Media / storage** | File search indexing |
| **Usage access** | Frequently used apps |
| **Device admin** | Uninstall protection |
| **Accessibility (App Locker)** | App lock intercept |
| **SMS** (optional) | SMS search / OTP |
| **Draw over other apps** (optional) | Floating OTP popup |

## Sensitive permissions explained

| Access | Why Dextera may ask |
|--------|---------------------|
| **Notification listener** | Custom notification center, badges, media awareness, OTP helpers |
| **Accessibility (Dextera App Locker)** | Detect when locked apps open so biometrics can be required |
| **Device admin** | Uninstallation protection (must be deactivated before uninstall) |
| **Usage access** | Frequently used apps |
| **SMS** | Optional SMS search and verification codes |
| **Display over other apps** | Optional floating OTP popup |

These are **optional** unless a feature requires them. Disabling them limits related features only.

## Manage permissions

- **Android Settings → Apps → Dextera → Permissions**  
- Notification access, usage access, accessibility, and device admin live under their own system settings areas  
- Feature toggles also exist inside **Dextera Settings**  

## Privacy note

Most processing stays on your device. Network is used only for optional features such as weather, Bing wallpaper, and web search suggestions. See the full [Privacy policy]({{ '/privacy/' | relative_url }}).
