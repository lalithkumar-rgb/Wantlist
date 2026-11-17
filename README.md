# WANTLIST v1.5.9 — Final Acquired Interaction

This consolidated GitHub Pages build preserves the existing WANTLIST data model and app features while adding the approved acquired-item interaction.

## What's included
- Subtle press-in/release feedback on **Mark as Acquired**.
- A lightweight card response as the acquired state appears.
- Celebration begins from the button's captured original screen position before the detail view changes.
- Five staggered particle waves with evenly distributed upward fan, a stronger returning/falling layer, ribbons, streamers, stars and confetti shapes.
- Theme-aware celebration palettes for Alpine, Forest, Coast, Desert Glow and Midnight Peaks.
- Acquired status and date shown in the detail view; the large action button is removed after acquisition.
- A reserved Undo icon slot immediately to the left of Edit. It fades in after acquisition while Edit and Delete remain in their existing positions.
- Undo returns the item to To Buy without another celebration or toast.
- Service worker cache version incremented to refresh deployed assets.

## Deploy
Upload the contents of this ZIP to the root of the existing GitHub Pages repository, replacing the matching files. Do not upload the ZIP itself.

## Files
- `index.html` — app and interaction changes
- `sw.js` — cache version update
- `manifest.webmanifest`
- `icon.svg`
- `apple-touch-icon.png`

Existing IndexedDB/localStorage data structures are unchanged. The app is not deployed automatically; upload the files to GitHub Pages to publish this build.
