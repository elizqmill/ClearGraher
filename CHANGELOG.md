# Changelog

All notable changes to ClearGraher are documented in this file.

## [1.0.4] - 2026-08-29

Updated to Telegraher 12.92.10 (build 6991010).

### Added
- Android 17 / GrapheneOS fixes (file sending, spacing, manifest intents).
- Unlimited file sending fix for high Android versions.

### Changed
- Base: Telegraher 12.92.9 → 12.92.10.
- Android 17/GrapheneOS compatibility fixes.
- ContactController package fix.
- Manifest update: missed intents.
- Monet theme improvements for Android 12+.
- Restrictions fix for messages (legacy).

### Removed
- Upstream's repeated attempts to re-add RU/IL restrictions (blocked).
- Upstream's repeated political renames in LoginActivity/BuildVars (blocked).

### ClearGraher (persists from 1.0.0)
- Restored RU and IL to login/registration country list.
- Removed political renames ("Slava Ukraini" / "Free Palestine").
- Neutralized `BuildVars.fuLabel`.
- App renamed to ClearGraher, links point to https://t.me/elizqmill.
- Own signing keystore in GitHub Actions secrets.

## [1.0.3] - 2026-08-29

Updated to Telegraher 12.92.9 (build 6991009).

### Added
- Unlimited multi-account: log in with the same phone number multiple times.
- TTL media flow in green and private chats: nudes last forever, screenshots allowed when PIN is enabled.
- "Kill the APP" button on profile to force-kill the app.

### Changed
- Base: Telegraher 12.92.7 → 12.92.9 (skipping 12.92.8 features merged together).
- Multi-acc: unlimited accounts with same phone number.
- TTL media: new flow for self-destructing media in secret/green chats, screenshots allowed with PIN.
- "Kill the APP" button on profile.

### Removed
- Legacy leftovers (CI/CD debug commits cleaned up).

### ClearGraher (persists from 1.0.0)
- Restored RU and IL to login/registration country list.
- Removed political renames ("Slava Ukraini" / "Free Palestine").
- Neutralized `BuildVars.fuLabel`.
- App renamed to ClearGraher, links point to https://t.me/elizqmill.
- Own signing keystore in GitHub Actions secrets.

## [1.0.2] - 2026-08-28

Updated to Telegraher 12.92.7 (build 6991007).

### Added
- Duress PIN code & new unlock flow (KABOOM after 10 fails, 3s retry delay).
- Monet themes: Light, Dark, AMOLED for Android 12+.

### Changed
- Base: Telegraher 12.92.6 → 12.92.7.
- PIN flow: retry delay 3s, KABOOM after 10 failed attempts.
- CI/CD: gradle caching and configuration cache fixed for forks.
- Removed Google Login and Google Vision libraries.
- Restrictions fix for messages (legacy fixes).
- XML cleanups.

### Removed
- Google Login.
- Google Vision.
- Legacy leftovers.

### ClearGraher (persists from 1.0.0)
- Restored RU and IL to login/registration country list.
- Removed political renames ("Slava Ukraini" / "Free Palestine").
- Neutralized `BuildVars.fuLabel`.
- App renamed to ClearGraher, links point to https://t.me/elizqmill.
- Own signing keystore in GitHub Actions secrets.

## [1.0.1] - 2026-08-21

Updated to Telegraher 12.92.6.

### Added
- Extended PIN flow: 4–16 digits (was fixed 4).
- PIN scramble re-randomizes layout on wrong attempts.
- Fingerprint unlock removed (so coercion can't bypass PIN).
- Gradle caching and configuration cache enabled (faster builds).

### Changed
- Base: Telegraher 12.92.5 → 12.92.6.
- App version bumped to 1.0.1 (build 6991006).

## [1.0.0] - 2026-08-19

Initial ClearGraher release, based on Telegraher 12.92.5.

### Added
- ClearGraher branding (app name, README, repo description).
- Own release signing keystore (stored in GitHub Actions secrets, never committed).
- Automated GitHub Actions build with universal APK.
- Changelog and SHA-256 checksum in release notes.

### Changed
- Removed country restrictions for registration/login (RU, IL) introduced by
  upstream Telegraher commits `43d56e4d9` and `1ea51984d`.
- Removed political renaming of countries in the login screen
  ("Slava Ukraini" / "Free Palestine").
- Neutralized `BuildVars.fuLabel`.
- Update channel link points to https://t.me/elizqmill.

### License
- Fork of Telegraher (GPL-2.0). This project is not affiliated with Telegram.