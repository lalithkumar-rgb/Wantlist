# WANTLIST v1.1 — GitHub Pages build

## Deploy
1. Create a GitHub repository named `wantlist`.
2. Upload every file in this folder to the repository root.
3. Open Settings → Pages → Deploy from a branch → `main` → `/ (root)`.
4. Open the HTTPS URL in Safari on your iPhone.
5. Tap Share → Add to Home Screen.

## Included
- Five selectable themes: Alpine Dawn, Forest Retreat, Coastal Calm, Desert Glow and Midnight Peaks.
- Adaptive, warm-light and dark appearance.
- Rotating landscape photography on Home.
- Editorial aspiration cover per item and a separate optional product-reference photo.
- Home, My List, Item Details, My Journey and Progress.
- Categories, priorities, estimated budget, actual paid amount, links and notes.
- Search, filtering, sorting, acquired history and move-back-to-list.
- IndexedDB persistence with migration from the earlier prototype's localStorage data.
- JSON export and restore.
- Starter list transcribed from the supplied Notes screenshot.
- Service-worker caching for the app shell and previously viewed Unsplash images.

## Photography
Theme and curated editorial images load from `images.unsplash.com`. These are passive image resources, not executable scripts. Previously viewed images may be cached for offline use; a first-time view requires internet. Uploaded product reference photos are stored locally and limited to 2.5 MB.

## Security and privacy
- No third-party JavaScript libraries, analytics, advertising SDKs or tracking pixels.
- Content Security Policy restricts scripts to this app, images to this app and Unsplash, blocks objects and external form actions.
- User-entered text is HTML-escaped before rendering.
- Product links open with `rel="noopener"`.
- Uploaded photos remain in local IndexedDB; they are not sent to a server.
- No account, cloud sync or backend.
- HTTPS is provided by GitHub Pages.

This is a local-first personal app, not a formally security-audited product. Browser storage is not encrypted by this app and may be lost if site data is cleared. Keep your iPhone protected, export backups, and do not store passwords, card numbers or other highly sensitive information.

## Starter data
The 24 entries from the supplied Notes screenshot are included. Four crossed-out items are pre-marked as acquired. The duplicate Power bank entry is intentionally preserved for you to review. No prices are invented.

## v1.1 iOS UI redesign
- Five complete themes, each with coordinated light/dark palettes applied to backgrounds, surfaces, cards, controls, navigation and supporting photography.
- iOS system typography, persistent high-contrast brand/settings bar, and a sticky back bar on item details.
- Bottom navigation is hidden during add/edit and item-detail flows so it cannot cover the content.
- Add/edit shows only item name, collection and priority first; optional budget, paid amount, link, cover photo, product photo, notes and status are grouped under More details.
- Removed the Home screen Up Next section and reduced repetitive motivational wording.

## PWA deployment and cache refresh in v1.1
- Service worker cache was bumped to `wantlist-v3`.
- Old service-worker caches are deleted during activation.
- App document and web manifest requests use network-first loading, with cached fallbacks for offline use.
- The app shell now precaches both the SVG app icon and the Apple touch icon.
- Web app name, description and launch colours were refreshed to match WANTLIST's updated design.
- After publishing, close the installed app completely and reopen it while online. If an old screen remains, remove the Home Screen shortcut and add it again after the site has loaded the new version.
