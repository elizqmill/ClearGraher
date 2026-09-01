# ClearGraher

**Our mission is to make sure what the Telegraher developer did never happens again.**

In 2026 the developer of [Telegraher](https://github.com/nikitasius/Telegraher) removed Russia (RU) and Israel (IL) from the login/registration country list — and renamed countries with political slogans inside the login flow.

**Ordinary users are not guilty** of the country they were born in, live in, have a phone number or an account from. A developer's personal dislikes must never decide who may use an app on their own device. Excluding people because of their passport or SIM code is discrimination, and this fork exists to prevent exactly that.

ClearGraher restores those countries and keeps them restored. Forever.

## Principles

* **No country-based exclusions** — every country stays in the login/registration list
* **No political renames** inside the app
* **This is my device** — no one gets to decide what i run on it, where i run my app, what must be deleted

## What it is

A fork of [Telegraher](https://github.com/nikitasius/Telegraher) (which is a fork of Telegram for Android), keeping its good parts: disabled ads, disabled remote deletions, save to gallery everywhere, full access in restricted chats, PIN scramble and more.

## Downloads

APKs are on the [releases page](https://github.com/elizqmill/ClearGraher/releases). Changelog: [CHANGELOG.md](CHANGELOG.md).

## BUILD

1) You clone the project on your dev laptop or a pc.
2) You run `gradle :TMessagesProj_AppStandalone:assembleStandalone` OR click in your IDE `TMessagesProj_AppStandalone -> assembleStandalone`
3) It will assemble for you APK and sign w/ default keys

## Links

* Github: https://github.com/elizqmill/ClearGraher
* TG channel: https://t.me/elizqmill

## License

GPLv2. See [LICENSE](LICENSE). Fork of Telegraher (GPLv2), which is a fork of Telegram for Android. Not affiliated with Telegram or Telegraher.
