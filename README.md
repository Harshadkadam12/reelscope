# Reelscope — ready-to-run PWA

## Run locally
1. Install Node.js 18+.
2. Open this folder in a terminal.
3. Run `npm install`
4. Run `npm run dev`
5. Open the URL Vite prints.

## Deploy
Upload the project to GitHub and import it into Vercel. Build command: `npm run build`. Output directory: `dist`.

For Vercel/Netlify SPA routes, configure fallback/rewrite to `/index.html` if your host doesn't automatically handle Vite client routes.

## Install prompt
The app includes:
- Web App Manifest
- HTTPS-compatible install flow
- custom `beforeinstallprompt` bottom install banner
- service worker
- responsive mobile UI

Browsers control whether `beforeinstallprompt` fires. It generally requires a secure deployed origin (HTTPS) and the browser's installability criteria. On iOS Safari, use Share → Add to Home Screen; the custom Android/Chromium prompt is not guaranteed there.

## Production note
The catalog is local demo data and uses placeholder image URLs. To publish a real movie discovery service, use a licensed metadata/image source (for example TMDB subject to its terms) and verify OTT availability before displaying provider claims.
