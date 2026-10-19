# Padel Battle website

Public landing page, support information, Privacy Policy, and Terms of Use for the
Padel Battle mobile app. This repository contains only the static website, not the
mobile app source code or user tournament data.

- Website: https://padel-battle.github.io/
- App Store: https://apps.apple.com/us/app/padel-battle-americano/id6775545020
- Google Play: https://play.google.com/store/apps/details?id=com.courtflow.padelbattle
- Support: urbanskyi.dev@gmail.com

## Files

- `index.html`: landing page and store links.
- `support.html`: contact information and frequently asked questions.
- `privacy-policy.html`: app data handling and Firebase disclosures.
- `terms.html`: Terms of Use.
- `style.css`: shared styles.
- `landing.css`: responsive landing page styles, separate from support and legal pages.
- `app-icon.webp`: 288 × 288 website icon, sized for the 96 px hero at up to 3× density.
- `favicon.png`: 64 × 64 PNG favicon.
- `app-icon.png`: original 1024 × 1024 icon, preserved without modification.

Keep the original icon intact; generate separate files for website optimisation.

## Landing page structure

1. App introduction and download links, with real tournament and standings screens.
2. Formats: Americano, Mexicano, fixed pairs, and Padel Battle.
3. Four steps: add players, play rounds, enter scores, and share results.
4. Common questions about accounts, offline use, fixed pairs, and platforms.
5. Download links, support, and legal pages.

The English landing page uses six real iOS screenshots. Original PNGs are preserved
alongside separate optimised WebP files under `assets/screenshots/ios/en/`; see
`assets/screenshots/README.md` for provenance and export details. Screenshots show
the iPhone app and are labelled as such. No Android screens or other localisations
are substituted into this first version.

The design retains the existing navy, teal, coral, system font, and light surfaces,
and introduces the app's court green for screenshot sections. Support and legal
pages continue to use the existing shared stylesheet.

The website has no JavaScript, forms, package dependencies, or build step.

## Preview and update

1. Create a branch for the change.
2. Edit the relevant HTML or CSS files. Keep privacy statements consistent across
   the landing page, support page, Privacy Policy, Terms, and store disclosures.
   Update the effective date when changing the policy or terms.
3. Preview locally with `python3 -m http.server 8000` and open
   http://localhost:8000/. Check the layout at desktop and phone widths, store
   links, navigation, and image loading.
4. Open a pull request against `main` and review the changes.
5. After merging, confirm that the GitHub Pages deployment succeeds and check the
   live website. GitHub Pages publishes from the root of `main`.

## Public repository hygiene

Keep this repository public for its GitHub Pages website. Never commit passwords,
tokens, private keys, signing files, local configuration, or user data.

For new commits, use the GitHub `noreply` email shown in your account's email
settings if you do not want to publish your personal email. Changing that setting
does not remove email addresses from existing commits.

Repository administrators should protect `main` against force pushes and deletion,
review write access, and check GitHub secret scanning alerts and push protection.
These are GitHub settings, not settings controlled by this website's files.

## Rights

Copyright © 2026 Ihor Urbanskyi. All rights reserved. This repository does not grant
an open-source licence for the website's code, text, or branding. GitHub's terms
continue to apply to viewing and forking the public repository.
