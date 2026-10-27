PNR 2026 — Ground Truth & Governance viewer

Place this whole pnr-2026-3d folder in the ROOT of your existing GitHub Pages repository. Do not replace the home page index.html.

Copy the "build" and "libs" folders from the downloaded Potree_1.8.2 distribution INSIDE pnr-2026-3d, alongside this index.html.

Expected layout:
repo-root/index.html       <-- your current home page (unchanged)
repo-root/pnr-2026-3d/index.html
repo-root/pnr-2026-3d/build/potree/potree.js
repo-root/pnr-2026-3d/libs/...

Point-cloud binary data remains on R2, and must NOT be copied into GitHub. The page is configured for:
https://pub-fa7300d8a7744ee9808d914e64643e3c.r2.dev/metadata.json

Test using https://YOUR-GITHUB-PAGES-URL/pnr-2026-3d/ . GitHub Pages will provide HTTPS. The page is deliberately unlinked from your home navigation, but is not private.

R2 CORS: permit your GitHub Pages origin, GET/HEAD, and Range header. Check in browser Network panel if remote loading fails.

This file provides DESKTOP Potree web viewing. QUEST 3 IMMERSIVE WEBXR IS NOT YET IMPLEMENTED; it can be added to this same HTTPS site after desktop loading and headset testing. No separate VR host required.

Note: This package does not include the Potree build/libs distribution, which you have already downloaded. If preferred, extract and copy those folders locally. This is a working integration candidate, not remotely end-to-end tested.
