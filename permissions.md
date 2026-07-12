---
title: Permissions
description: Why Dextera asks for each Android permission or system access — including Accessibility for App Locker.
permalink: /permissions/
---

Dextera only uses permissions needed for features you enable. Optional items can be deferred and enabled later in Settings or system Settings.

## Why Dextera uses Accessibility {#accessibility}

Dextera is **not** an accessibility tool for users with disabilities. The optional **Dextera App Locker** accessibility service exists only for **security**: app locking with biometrics or your device credential.

| Topic | Detail |
|-------|--------|
| **Why** | Android does not provide a public API that reliably intercepts when a specific app opens (including from Recents). Accessibility is the supported system mechanism that lets Dextera detect a locked app coming to the foreground. |
| **What it does** | Watches for locked apps opening, shows an opaque cover so content is not readable under the prompt, and requires biometric / device credential before the app is usable. |
| **What it does not do** | Read passwords, keystrokes, or form fields; control other apps; scrape screen content for ads or analytics; send accessibility events or locked-app data off your device. |
| **When it runs** | Only if you enable **Global app locker** and turn on the **Dextera App Locker** service in system Accessibility settings. Turn the service or feature off anytime to stop it. |

**Purpose (plain language):** fraud prevention / security and compliance — keep selected apps private until you unlock them on this device.

This page is the public disclosure for that use of Accessibility. Related: [Privacy policy — sensitive permissions]({{ '/privacy/#accessibility-device-admin-and-sensitive-permissions' | relative_url }}) and [Features — Global app locker]({{ '/features/' | relative_url }}).

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
| **Accessibility (App Locker)** | [App lock intercept](#accessibility) |
| **SMS** (optional) | SMS search / OTP |
| **Draw over other apps** (optional) | Floating OTP popup |

## Sensitive permissions explained

| Access | Why Dextera may ask |
|--------|---------------------|
| **Notification listener** | Custom notification center, badges, media awareness, OTP helpers |
| **Accessibility (Dextera App Locker)** | Detect when locked apps open so biometrics can be required — [full explanation](#accessibility) |
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
