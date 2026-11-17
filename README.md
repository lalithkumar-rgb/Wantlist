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

## v1.2 UI refinements
- Rebuilt bottom navigation with aligned inline SVG icons and a translucent Liquid Glass treatment.
- Removed duplicate theme access from My List; global settings remains in the persistent app header.
- My List now has a single-line search and filter control. Status, collection and sort options are grouped in one filter sheet with Apply and Reset.
- Removed generic category stock thumbnails; only exact known product imagery is used, otherwise a designed typographic cover appears until a personal product photo is added.
- Edit and delete actions sit beside the item name; redundant lower actions removed.
- The WANTLIST brand and Settings remain fixed at the top on every screen.
- Service worker cache bumped to wantlist-v4.

## v1.3 — Home, Collections & Interaction Refinement
- Added global bottom safe-area clearance so final content on Home, My List, Journey and Progress can scroll above the floating navigation.
- Home progress summary is now a theme-aware, lower-emphasis interactive card that opens Progress.
- Collection tiles and Progress breakdown use user-managed collections.
- Collections can be created, renamed, and deleted with item reassignment confirmation. Renaming updates existing items. Collections persist separately from themes and are included in backups.
- Add/Edit suggests a collection from the item name and allows manual override.
- Added curated, item-relevant cover suggestions in the item editor plus local photo upload support.
- Add/Edit action bar is now a differentiated Cancel + Save row. Save activates after edits; status options stay on one line.
- Expanded More Details is visually grouped and uses the same type scale and control styling as the rest of the editor.
- Mark as Acquired uses a more prominent theme-aware action and a short confetti burst only (no congratulatory text). Respects Reduce Motion.
- Service worker cache bumped to `wantlist-v5`.


## v1.4 refinement update

- Home progress summary now uses the selected minimal horizontal progress-bar design.
- Item detail pages reset to the top when opened.
- More Details remains one expandable section, with optional fields organized into subtle card groups (Option E).
- Add/Edit action buttons are fixed to the bottom safe area; form content scrolls above them and ends before the footer.
- Main navigation content clearance is increased so the final list cards can scroll fully above the floating navigation.
- Acquisition confetti now originates only from the Mark as Acquired button on the item detail page, falls across the screen for approximately 3.4–4.0 seconds, and fades out. List checkboxes do not trigger confetti. Reduce Motion is respected.
- Service worker cache updated to wantlist-v6.

Source validation: JavaScript syntax and manifest JSON checked. Please test on iPhone Safari/Home Screen after deploying; this build has not been device-tested.
\n\n## v1.5 refinement\n- Mobile-first single-column More Details layout; two columns only on wider screens.\n- Reduced bottom scroll clearance while retaining safe space for floating navigation.\n- Journey focuses on milestones; duplicate statistics removed.\n- Removed repeated item-count labels from Home and My List.\n- Home collection tiles open dedicated collection views with search and live item counts.\n- Theme-aware Big Burst confetti, triggered only by Mark as Acquired.\n- Service worker cache updated.\n

## v1.5.1 corrections
- Rebuilt confetti CSS and trajectory for a true upward semicircular burst followed by gravity; burst originates at the Mark as Acquired button.
- Removed the duplicate filtered item count below the My List search row; the header count remains.
- Cover picker is now an image-only horizontal scroller with up to eight suggestions; labels removed.
- Service worker cache updated to wantlist-v8.


## v1.5.3 consolidated build
- Integrated the approved Big Burst v2 celebration with theme-specific palettes and reduced-motion support.
- Retained robust collection tile navigation and collection item search/detail navigation.
- Refined the floating bottom navigation dock sizing, readability, and iPhone safe-area positioning.


## v1.5.4 Consolidated Release
- Celebration effect rebuilt for a faster, denser, multi-wave surprise burst with varied confetti, ribbons, and streamers.
- Midnight Peaks refined with layered midnight navy, blue-slate surfaces, and champagne accents in light and dark appearance.
- Floating bottom navigation enlarged and repositioned with improved labels, icons, and iPhone safe-area spacing.
- Collection navigation fix retained from v1.5.2/v1.5.3.


## v1.5.5 Celebration refinement
- Reworked the acquired celebration for a denser immediate burst, stronger outward velocity, larger foil/confetti/ribbons/streamers, a brief shock ring, and a quick secondary volley.
- Tuned the effect for an approximately 2.5–3 second finish while retaining theme palettes and iOS Reduce Motion support.
- All v1.5.4 collection navigation, dock, and Midnight Peaks refinements are retained.
