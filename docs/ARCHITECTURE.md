# Architecture

## Legacy Problem
The older Spartan / Ryan Bot stack mixed too many runtime layers:

- Electron shell
- managed Chrome profile
- Chrome tab orchestrator
- Chrome extension
- Facebook tab

That made communication brittle and state easy to lose.

## Warhawk Direction
Warhawk should simplify the stack to:

1. web app
2. orchestrator tab
3. Chrome extension
4. Facebook tab

## Why Keep The Orchestrator Tab
The orchestrator tab is a deliberate control boundary.

- It keeps runtime activity visible.
- It gives the operator a place to understand what is happening.
- It helps preserve a more human browser cadence.
- It is part of the anti-ban strategy.

The goal is not to hide more automation. The goal is to keep the runtime simpler and safer.

## What Gets Removed
- Electron as the operator shell
- localhost relay patterns between app shell and Chrome
- Spartan-specific packaging and branding

## What The Web App Owns
- auth
- settings
- queue truth
- inventory
- collateral
- listing composition
- download and onboarding guidance

## What The Extension Owns
- Chrome APIs
- browser tab control
- Facebook DOM interaction
- runtime execution inside the operator browser

## Design Rule
Remove Electron complexity, but keep the visible tab-based orchestration model if that is what keeps the runtime safer and less bot-like.
