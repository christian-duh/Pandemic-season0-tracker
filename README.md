# Pandemic Legacy: Season 0 Field Tracker v7 — ALL MONTHS UNLOCKED

This build removes every month gate. Prologue and January through December can be selected at any time.

## Important behavior
- All months are selectable during setup.
- You can switch the active month during a live tracked game without clearing board/deck state.
- Older v6 August-safe browser saves are migrated automatically when hosted at the same origin.
- All Campaign Tools are always available for branch-dependent or copy-specific mechanics.
- Satellite cards keep unknown identities separate from known pile locations.
- Autosave, snapshots, Undo, JSON backup/import, recovery links, mobile and desktop layouts remain.

## Updating an existing GitHub Pages install
Replace the existing repository root files with the contents of this folder and commit to your Pages branch.
The v7 service worker is network-first for the app shell, so future `index.html` updates should refresh more reliably.
Inside the app, **Save → Check for app update** forces a service-worker update check and reload without deleting local game state.

## Files
Upload these to the repository root:
- index.html
- manifest.webmanifest
- sw.js
- icon-192.png
- icon-512.png
- .nojekyll

The physical game materials remain authoritative for objective wording, story branches, and exact instructions that vary by campaign state.
