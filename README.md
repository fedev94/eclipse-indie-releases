# Eclipse Indie Releases

Public update feed for **Eclipse Render Manager Indie** desktop releases.

This repository contains **binary installers and auto-update metadata only**.
It does **not** contain application source code.

## Purpose

The desktop app (`electron-updater`, generic provider) reads update metadata from this repository and downloads the newest installers.

Feed URL used by the app:

`https://raw.githubusercontent.com/fedev94/eclipse-indie-releases/main`

## Required files in repository root

For updates to work, publish these files from each release build to the root:

- `latest.yml` (Windows metadata)
- `latest-mac.yml` (macOS metadata)
- Windows installer artifacts (`*.exe`, optional `*.blockmap`)
- macOS artifacts (`*.zip`, optional `*.dmg`)

## Notes

- Keep this repo focused on release artifacts only.
- Do not upload private keys, tokens, or source code.
- The app still enforces license checks separately.
