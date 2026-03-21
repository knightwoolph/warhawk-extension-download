# Onboarding Flow

This is the operator onboarding sequence the Warhawk web platform should ultimately guide.

## Operator Flow
1. Log into the Warhawk web app.
2. Go to the extension setup / download surface.
3. Download the current extension package.
4. Open `chrome://extensions`.
5. Enable `Developer mode`.
6. Load the unpacked extension folder.
7. Pin the Warhawk extension.
8. Open the dedicated orchestrator tab.
9. Confirm the Facebook session is logged in and usable.
10. Return to the Warhawk web app and verify setup is complete.

## What The Web App Should Explain
- the extension is separate from the web app
- the operator must install it in Chrome manually during dev rollout
- the orchestrator tab is a required part of the runtime, not an optional oddity
- Facebook actions happen in browser tabs, not only in the web dashboard

## What Good Onboarding Looks Like
- short checklist
- version guidance
- troubleshooting links
- clear next actions
- honest explanation of what the extension does

## Future Nice-To-Haves
- setup progress checklist in the web app
- version detection / heartbeat
- direct "open orchestrator tab" action once installed
