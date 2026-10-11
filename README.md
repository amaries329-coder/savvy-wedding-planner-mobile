# Savvy Wedding Planner — mobile source v0.1

Prepared Android and iOS Capacitor projects, with a compiled bundled web interface.
This is source code, not an APK, AAB, IPA, or store-approved release.

## Included
Wedding profile and countdown, checklist, budget, guest RSVPs, vendor contacts,
wedding-day timeline, notes, manual on-device saving, backup import/export UI,
and device-data deletion. Core planning works offline without signing in.

## Build
Requires Node 22+, npm, Android Studio/SDK for Android, and a Mac with Xcode for iOS.
Run `npm ci`, `npm run build`, and `npm run sync`.
Run `npm run android` to open Android Studio, or `npm run ios` on a Mac to open Xcode.
Android: configure the SDK and release keystore, then build a signed Android App Bundle.
iOS: select your Apple developer team and unique bundle identifier, archive, and upload.
Provisional bundle identifier: org.savvyweddingplanner.app.

## Verified here
Production web build succeeded; Capacitor generated and copied bundled assets to
both native projects. No native compilation, simulator, or physical-device test
was possible in this workspace. No release signing keys were created.

## Remaining before a store release
- Compile native projects and test on Android and iPhone, including data persistence,
  safe areas, keyboard, backup export/import, external links and device deletion.
- Replace generated default app icons and launch assets with approved branding.
- Review local-data privacy policy and complete accurate store privacy declarations.
  Linked website policy describes the website; it needs mobile-specific review.
- Configure developer accounts, signing, listings, screenshots, and required testing.
- Store review and approval.

## Scope and limits
Data is stored only in this app on this phone using localStorage; it does not sync
with the website or the ChatGPT account. Uninstalling/clearing app data may remove it.
Save changes before closing. Backup download uses a browser-style Blob link and
must be verified on devices; native file sharing is not yet integrated.
Paid subscriptions, premium tools, website sign-in, and cloud synchronization are
not included in this first mobile version. Subscription integration requires a
separate store-payment and entitlement implementation.
