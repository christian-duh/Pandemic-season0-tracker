# Season 0 Tracker — start-from-scratch version

This version intentionally starts with a blank setup screen. No game state, city list, removed card, player names, or month-specific campaign information is preloaded.

## Autosave
After you press **Start tracker**, the app:
- saves after every game action
- saves again when you leave/switch apps
- keeps up to 30 recent snapshots for Undo / recovery
- can export and import a JSON backup
- can create a recovery link containing the full current game state

## Files to upload to GitHub
Upload these files to the root of one repository:
- `index.html`
- `manifest.webmanifest`
- `sw.js`
- `icon-192.png`
- `icon-512.png`
- `.nojekyll`

You can also upload this README, but it is optional.

## GitHub Pages
In the repository:
1. Open **Settings**.
2. Open **Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Choose branch **main** and folder **/(root)**.
5. Save.
6. Wait for the Pages URL to appear, then open it in Safari.
7. In Safari, choose **Share → Add to Home Screen**.

The site can work offline after it has loaded successfully once.
