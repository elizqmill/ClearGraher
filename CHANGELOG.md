# Changelog

All notable changes to ClearGraher are documented in this file.

## [1.0.0] - 2026-08-19

Initial ClearGraher release, based on Telegraher 12.92.5.

### Added
- ClearGraher branding (app name, README, repo description).
- Own release signing keystore (stored in GitHub Actions secrets, never committed).
- Automated GitHub Actions build with per-architecture APKs:
  - armv7 (32-bit)
  - arm64-v8a (64-bit)
  - x86 (32-bit)
  - x86_64
  - universal (all architectures)
- Changelog and per-file SHA-256 checksums in release notes.

### Changed
- Removed country restrictions for registration/login (RU, IL) introduced by
  upstream Telegraher commits `43d56e4d9` and `1ea51984d`.
- Removed political renaming of countries in the login screen
  ("Slava Ukraini" / "Free Palestine").
- Neutralized `BuildVars.fuLabel`.
- Update channel link points to https://t.me/elizqmill.

### License
- Fork of Telegraher (GPL-2.0). This project is not affiliated with Telegram.