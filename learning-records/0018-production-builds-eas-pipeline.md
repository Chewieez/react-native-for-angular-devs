# Learning Record 0018: Production Builds & EAS Pipeline

## Date: 2026-08-14

## Key Insight
1. **Compilation vs Bundling**: Mobile production requires compiling signed binary artifacts (`.ipa` / `.aab`) rather than static web bundles.
2. **EAS Build**: Multi-profile compilation (development client, internal preview, production) defined cleanly in `eas.json`.
3. **EAS Update (OTA)**: Push instant JavaScript and asset updates to user devices Over-The-Air, bypassing standard App Store review delays for fast bug fixes.

## Application to Codebase
- Define bundle identifier, splash screen, and permissions in `app.json`.
- Configure build profiles in `eas.json` for testing and store release.
