# Changelog

All notable changes to ClearGraher are documented in this file.

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
