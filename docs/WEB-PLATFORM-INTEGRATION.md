# Web Platform Integration

The web platform should expose extension setup as a first-class operator workflow.

## Required Web Responsibilities
- provide a download CTA for the current extension package
- explain that the extension is a separate install
- show step-by-step setup instructions
- explain how to open `chrome://extensions`
- explain `Load unpacked`
- guide the operator to the orchestrator tab
- explain how to verify Facebook readiness
- link to troubleshooting docs

## Recommended Surface Areas In The Web App
- settings
- queue
- a dedicated extension setup / download route
- onboarding entry after first login

## Messaging Rules
- be honest about the install path
- do not pretend it is a one-click browser-store install if it is not
- explain why the orchestrator tab exists
- explain that the extension is part of the browser runtime, not a dashboard widget

## Future Product Hooks
- installed version display
- last heartbeat / last runtime check-in
- warning when extension is not connected
- direct link to release notes
