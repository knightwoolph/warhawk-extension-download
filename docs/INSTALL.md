# Install Guide

## Development Install
Use this flow while the extension is still being developed and tested outside the Chrome Web Store.

1. Download or unpack the latest Warhawk extension build.
2. Open `chrome://extensions`.
3. Enable `Developer mode`.
4. Click `Load unpacked`.
5. Select the unpacked extension folder.
6. Pin the Warhawk extension in Chrome.
7. Sign in to the Warhawk web platform.
8. Follow the extension onboarding steps from the web app.

## What Operators Need
- a Chrome profile dedicated to Warhawk operations
- access to the Warhawk web platform
- access to the relevant Facebook account/session
- the current extension package from this repo's release channel

## What The Web App Should Tell Them
- where to download the extension
- how to load it in Chrome
- how to confirm it is active
- how to open the orchestrator tab
- how to verify Facebook is ready before running queue work

## Current Packaging Assumption
Until a store-based delivery path exists, package distribution is manual and explicit:

- unpacked folder for local development and QA
- zipped release package for operator download when needed

## Notes
- Manual install via `chrome://extensions` is the default development path.
- Do not require Electron for install or runtime.
