# Warhawk Extension Download

Distribution repo for the Warhawk Chrome extension.

This repo is separate from the main web platform on purpose. The web app is the system of record and operator console. The extension is a separate browser runtime that operators download and install.

## Why This Repo Exists
- keep release packaging separate from the web app repo
- host install docs and onboarding docs in one place
- support manual developer-mode installs through `chrome://extensions`
- prepare a clean handoff path from the web platform download surface to the extension package

## Source Repositories
- Web platform and current extension source:
  - `C:\Users\eumst\project\warhawk-platform`
- Legacy Spartan / Ryan Bot source to mine:
  - `C:\Users\eumst\project\Ryan Bot`
  - `C:\Users\eumst\project\Ryan Bot\extension`

## Runtime Model
Warhawk should use this browser runtime shape:

1. web app
2. orchestrator tab
3. Chrome extension
4. Facebook tab

The separate orchestrator tab is intentional. It keeps the runtime visible, operator-observable, and closer to a human browser workflow.

## Repo Contents
- `docs/INSTALL.md`
  - manual install steps for development and operator testing
- `docs/ONBOARDING.md`
  - onboarding sequence the web platform should mirror
- `docs/ARCHITECTURE.md`
  - browser runtime design and anti-ban rationale
- `docs/WEB-PLATFORM-INTEGRATION.md`
  - what the web app must expose for download, setup, and support
- `release-manifest.json`
  - placeholder manifest for tracking current release metadata
- `releases/README.md`
  - release storage expectations

## Current Delivery Assumption
- development install is manual via `chrome://extensions`
- operator onboarding should be initiated from the Warhawk web app
- Chrome Web Store distribution is future scope, not required for the first Warhawk rollout

## Initial Release Workflow
1. Build the extension from the main Warhawk source repo.
2. Produce a versioned package or unpacked folder.
3. Publish release notes and metadata here.
4. Point the web platform download/install docs to the new release.

## Next Work
- rebrand Spartan assets to Warhawk
- rewire the extension away from Electron assumptions
- define the orchestrator tab behavior cleanly
- add the web-platform download and onboarding route
