# Warhawk Extension

Chrome extension for Facebook Marketplace posting automation.

## Install

1. Download this repo (Code > Download ZIP, or `git clone`)
2. Go to `chrome://extensions`
3. Enable **Developer mode** (top right)
4. Click **Load unpacked**
5. Select the `extension/` folder from this repo
6. Done — the Warhawk icon appears in your toolbar

## Update

1. Pull latest (`git pull`) or re-download
2. Go to `chrome://extensions`
3. Click the reload icon on the Warhawk card

## Current Version

**v1.7.1** — 2026-03-22

See [release-manifest.json](release-manifest.json) for full changelog.

## Structure

```
extension/          <-- Load this folder in Chrome
  manifest.json
  background/       Service worker (queue processing, heartbeat)
  content/          Form detector + filler (injected into FB Marketplace)
  delete-handler/   Delete automation (injected into FB listing pages)
  popup/            Extension popup (login, status)
  orchestrator/     Orchestrator tab (anti-ban runtime surface)
  bridge/           SaaS <-> extension communication bridge
  icons/            Extension icons
```

## Source

Built from [warhawk-platform/extension](https://github.com/knightwoolph/warhawk-platform/tree/master/extension).
