# Season 0 Field Tracker — v6 August-Safe

This build is intentionally spoiler-safe beyond **August**. It contains tracker logic only for mechanics your group can have encountered by the beginning of / during August. September–December appear only as locked calendar month names; no later mechanic names, rules, components, objectives, or story data are encoded.

## August readiness
The August profile keeps all previously unlocked tracking active and adds a lightweight personnel/alias loadout area for the physical character additions your group has actually revealed. It also exposes the post-July satellite-control workflow without preloading hidden card or story text.

The physical Legacy deck, Operations cards, Debrief Book, opened boxes/doors, and your actual campaign choices remain authoritative. The app deliberately does not reproduce hidden objective/story text.

## Major v6 fix: unknown Satellite identities
The previous July build incorrectly asked you to assign each Satellite Launch **region identity** to a specific Player-deck pile even when the setup only told you which piles contained a Satellite card.

v6 separates those facts:

1. Enter the **remaining Satellite identities** as one unordered region pool.
2. Enter only the **number of Satellite cards hidden in each of the five Player-deck piles**.
3. Do not guess which identity is in which pile.
4. When a Satellite Launch is actually drawn, choose the region shown on the physical card. The app removes that identity from the remaining pool and one hidden Satellite slot from the current pile.

Example: if three unknown Satellite cards are shuffled one each into piles 3, 4, and 5, enter the three possible regions in the pool and use pile counts `0, 0, 1, 1, 1`.

The next-draw Satellite probability now uses the pile counts while identity probabilities remain unresolved until reveal.

## Core tracker features
- Month profiles from Prologue through **August**; later months hard-locked.
- Guided 9-city opening Threat setup (3/3/3, 2/2/2, 1/1/1 agents).
- Full city autocomplete with common alternate spellings.
- Player-deck five-pile model with Escalation odds.
- Satellite Launch probability and reveal tracking using unknown identities correctly.
- Threat deck modeled as shuffled layers, discard, Game End area, removed cards, and exact known top order.
- Separate regular Threat and Infection card modeling.
- City agent counts, Incidents, disease cubes/outbreaks, surveillance, safehouses, pursuit/checkpoints, teams, and related board notes.
- Risk dashboard showing current-draw and conditional post-Escalation city/Incident probabilities.
- Campaign modules for already-unlocked trials, infiltration/security, satellites, objectives, and August personnel/loadout notes.
- Generic funded/special-effect tools for known order, card removal, skipped Threat stage, and manual deck corrections.
- Active Satellite state plus a **Disable active satellite** control; keep the physical-board temporary surveillance city list synced after using it.
- Autosave after every change, Undo, up to 40 snapshots, backup import/export, and recovery URLs.
- Responsive phone UI plus wider desktop command-center layout.

## Upgrading your existing GitHub Pages app
Replace the repository-root files with the files in this package:

- `index.html`
- `manifest.webmanifest`
- `sw.js`
- `icon-192.png`
- `icon-512.png`
- `.nojekyll`

Commit to the same branch used by GitHub Pages. The service-worker cache name is bumped to `s0-field-august-v6`, so reopen/refresh the site once before relying on offline mode.

### Existing v5.1 local state
v6 will attempt to import the prior v5.1 browser state automatically when running at the same GitHub Pages URL. Old Satellite pile identities are intentionally converted into an **unassigned hidden identity pool** while preserving the number of hidden Satellite cards in each pile. This removes any false certainty created by the old setup model.

## Campaign progression reminder
Use your recorded evaluation / Debrief calendar to confirm which month you are actually starting. The tracker does not guess campaign progression when the physical record disagrees.
