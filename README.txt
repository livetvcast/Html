DIRECT VIDEO LINK FINDER — AppMint + Vercel
==========================================
Files:
- index.html: AppMint HTML/WebView app UI
- api/extract.js: Vercel API scans public HTML, same-origin iframe and linked JS for common media URLs
- package.json

SETUP
1) Extract ZIP.
2) Upload index.html, package.json and api/extract.js to a GitHub repository.
3) Import repository into Vercel and Deploy.
4) In index.html, replace https://YOUR-PROJECT.vercel.app/api/extract with your actual Vercel deployment URL plus /api/extract.
5) Import index.html into AppMint using its HTML/WebView project option and build APK.

IMPORTANT
- Static HTML apps usually cannot fetch arbitrary websites because of browser CORS. The Vercel API is needed for website URL scan.
- This is best-effort, not a universal extractor. It scans HTML, same-origin iframes and some linked JS files; it does not run the site's player or capture all live network requests.
- Login walls, anti-bot systems, cross-origin iframes, signed/temporary URLs, DRM/encrypted streams and private content may not work. Use only content you own or are authorized to access.
- M3U8/MPD are stream manifests, not necessarily MP4 files.
- This ZIP is project source, not a prebuilt APK. AppMint's import/build process is still required.
