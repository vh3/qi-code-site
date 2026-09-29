# MorsePath marketing/legal site (published)

> The app was renamed from "Qi Code" to "MorsePath" (owner decision, 2026-09-08, see `DECISIONS.md` F78). The site repo, its URL slug (`qi-code-site`), and the file paths below intentionally still say "qi-code" -- those are live, already-verified App Store Connect URLs and renaming the repo would break them for no user-visible benefit. Revisit only if the site content itself needs a refresh.

> **Published 2026-08-26** to [vh3/qi-code-site](https://github.com/vh3/qi-code-site) — public, GitHub Pages from `main` root, HTTPS enforced. Live and verified:
> - https://vh3.github.io/qi-code-site/privacy.html
> - https://vh3.github.io/qi-code-site/support.html
>
> These files are the mirror kept alongside the app. The deployed copies live in that repo; if you edit here, copy the changed files over and push, or edit there and re-copy back.


These pages exist to satisfy two App Store Connect fields that are **hard blockers** for the listing: **Privacy Policy URL** and **Support URL**. Apple requires a privacy policy URL even for an app that collects nothing.

They are written to match the sibling `nineby-go-site` in structure, tone, and stylesheet, so the two apps look like they come from the same publisher. `styles.css` is copied verbatim from that site.

## Files

| File | Purpose |
|---|---|
| `index.html` | Small landing page, linked from the other two |
| `privacy.html` | Privacy Policy → the Connect **Privacy Policy URL** |
| `support.html` | Support page with contact and common questions → the Connect **Support URL** |
| `styles.css` | Shared stylesheet (copied from `nineby-go-site`) |

English only, matching the app. Do not add localized pages unless the app itself is localized — Nineby had to reconcile exactly that mismatch during review.

## How it was published

Followed the `nineby-go-site` pattern exactly: public repo under `vh3`, files at the repo root, GitHub Pages serving `main` / root with HTTPS enforced. Only the site repo was pushed — the app repository is still local-only.

To update a page: edit it in the site repo, commit, push. Pages rebuilds in under a minute.

## Still worth confirming

- The support email `bfgames.support@gmail.com` is correct for this app (copied from Nineby Go).
- **Publisher name updated 2026-09-29:** the public-facing name in these pages is now spelled out as "Brain Fart Games" rather than the bare initialism "BFG" -- a real company, BF Games, was found to already exist under that abbreviation, and the owner asked for the full name instead of switching to a personal name. This has NOT been reconciled with (a) the sibling `nineby-go-site`, which still says "BFG" as of this note, so the two sites will now read as different publishers until that one is updated too, and (b) whatever name Apple's own "Seller" field shows on the App Store product page for this developer account, which is an Apple Developer Program account-level setting, not something a site-content edit changes. **Also flagged, not yet acted on:** the support email address below, `bfgames.support@gmail.com`, itself reads as "BF Games" right next to the domain -- the exact collision this rename was meant to avoid. Left unchanged pending the owner's decision, since it is a live, shared inbox also used by the sibling Nineby Go app.
- The privacy page's description of stored data still matches `LocalStore.swift`. It currently describes: settings, per-character practice evidence, individual attempt records, and recent session summaries.

## Keep in sync

If a future release adds accounts, cloud sync, advertising, or analytics, `privacy.html` must be updated **and** the App Privacy nutrition labels in Connect redone before that build ships.
