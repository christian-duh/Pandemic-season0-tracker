# Season 0 Field Tracker — v5.1 July-Safe

This build is intentionally spoiler-safe beyond **July**. It contains tracker logic only for mechanics available through July. August–December appear only as locked month names; no future mechanic names or rules are embedded.

## What changed
- July Satellite Launch cards can be assigned to the physical Player-deck piles during setup.
- The Turn screen calculates the chance that the next Player draw contains a Satellite Launch in addition to Escalation odds.
- Recording a Satellite Launch consumes the correct modeled Player-deck card and tracks the active region.
- July Satellite Watch stores active regions, temporary-surveillance city lists, control-center/bug notes, and remaining launch cards by pile.
- Prologue through July are available in the month dropdown; later months are hard-locked.
- The app still supports 9-city opening setup, agent/incident risk, conditional post-Escalation risk, disease board-state notes, pursuit/checkpoints, infiltration/security, city autocomplete, active-team Mop Up, autosave, snapshots, backups and recovery links.
- New responsive desktop command-center layout, while keeping the phone UI compact.

## GitHub Pages upgrade
Replace your repository's existing `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`, and `.nojekyll` with the files in this ZIP. Commit the changes. GitHub Pages will redeploy automatically. Because the service-worker cache name changed, reopen/refresh the site once before relying on offline mode.

## Important setup note for July
Follow the physical July setup instructions for where each Satellite Launch card is placed. Then enter each card's **region** under the matching Player-deck pile in the app. The app does not guess the distribution.

## Future months
This version deliberately does not contain future-month mechanics. When you reach the next month, update the app with a new month profile; the architecture is set up so the existing campaign/game state can continue.


## v5.1 disease-card accuracy
From the disease module onward, Infection cards are modeled as a distinct card type rather than as duplicate regular Threat cards. In manual deck-correction fields, type `I:Toronto` for an Infection card and simply `Toronto` for a regular Threat card. The risk screen separates agent/Incident probability from disease/outbreak probability.
