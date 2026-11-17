# WANTLIST v1.6.0 — Final Consolidated Build

Production update based on the approved v1.6.0 behavior and the selected **Option A — Balanced** item-details layout.

## Item details — Option A
- Retains the single large product image at the top; removes the duplicate “Your product photo” block.
- Keeps the item title and action controls in their existing positions.
- Shows Acquired / To Buy status near the top.
- Groups estimated budget and actual amount side by side under Purchase overview.
- Shows a savings / budget-overrun indicator when the item is acquired and both amounts are available.
- Groups the product link and optional notes under Product information.
- Preserves the sage-green visual identity and responsive light/dark themes.

## Other v1.6.0 changes retained
- Purchase confirmation sheet with an optional actual-amount field.
- Actual amount is retained when an item is moved back to To Buy and acquired again.
- The item's uploaded product image takes priority in My List cards and Journey entries.
- Product-link review affordance and manual fallback guidance for stores that block automated metadata access.
- Existing celebration animation and interaction are retained.

## Data safety
- Startup uses the existing `initialiseData()` path.
- No preview/sample item is injected and no existing item list is replaced.
- Existing IndexedDB/localStorage data model and backup format are retained.
- Export a JSON backup before deploying an app update.

## Deployment
Upload the contents of this folder to the root of the existing GitHub Pages repository, replacing the previous app files. Keep filenames and directory structure unchanged. The service-worker cache name has been advanced so the updated app assets are fetched after deployment.

## Product metadata limitation
The Find product details control validates the URL and explains the lookup limitation; it does not perform live retailer scraping. A compatible metadata service is required for reliable automatic title, image, and price extraction.
