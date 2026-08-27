# Qi Code — public site

Public static pages for **Qi Code** (subtitle: Morse Trainer) App Store / TestFlight fields:

| Page | Path | Purpose |
|---|---|---|
| Home | [`index.html`](index.html) | Short product blurb |
| Support | [`support.html`](support.html) | Support contact — App Store **Support URL** |
| Privacy | [`privacy.html`](privacy.html) | Privacy Policy — App Store **Privacy Policy URL** |

**Support email:** bfgames.support@gmail.com

English only, matching the app. Qi Code's iPhone UI is English in Version 1, so
these pages are not localized either — unlike the sibling `nineby-go-site`,
whose app localizes to French and German.

## Why this repo is public

Apple requires a reachable privacy policy URL for every App Store listing, even
for an app that collects no data — Qi Code makes no network calls at all. GitHub
Pages needs a public repository to serve these pages for free. The iOS
application source stays private.

## Published at

- https://vh3.github.io/qi-code-site/
- https://vh3.github.io/qi-code-site/privacy.html
- https://vh3.github.io/qi-code-site/support.html

Served by GitHub Pages from `main`, root folder, HTTPS enforced. Styling matches
`nineby-go-site` so both apps read as the same publisher.

## Keeping it accurate

`privacy.html` describes what the app stores on the device: settings,
per-character practice evidence, individual practice attempts, and recent
session summaries. If a future release adds accounts, cloud sync, advertising,
or analytics, update that page **and** redo the App Privacy nutrition labels in
App Store Connect before the build ships.

Source of truth for the listing itself lives with the app, in
`MorseCodeTrainer/docs/store/`.
