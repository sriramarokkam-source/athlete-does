# ATHLETE DOES — Installable Android PWA

A self-contained progressive web app for hammer throw, strength records, training checklists/calendar, performance charts, nutrition/body weight, recovery and study planning.

## Easiest free setup: GitHub Pages

**A PWA must be served from HTTPS to install correctly.** Opening `index.html` as a local file is not enough. GitHub Pages gives your app an HTTPS address.

1. On your phone or computer, sign in or create a GitHub account at https://github.com.
2. Create a new repository named `athlete-does` (Public is simplest for free GitHub Pages).
3. Upload the files and folders from this ZIP. The `index.html` file must be in the repository root, alongside `manifest.json` and `sw.js`; upload the `icons` folder too.
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/(root)`, then Save.
6. Wait for GitHub Pages to publish. Your address will look like `https://YOUR-USERNAME.github.io/athlete-does/`.
7. Open that HTTPS address in Chrome on Android. Open Chrome's **⋮** menu and tap **Install app** or **Add to Home screen**. Confirm.
8. Launch ATHLETE DOES from the new home-screen icon. Once loaded, the core app works offline after the first successful load.

## What is included

- `index.html` — app and UI
- `manifest.json` — install name, standalone display, theme and icon references
- `sw.js` — service worker for offline caching
- `icons/` — 192px and 512px app icons plus SVG source

## Data storage and backup

Workout data is stored in the browser's localStorage for the deployed site origin. It stays on this device/browser, not in a cloud account. Export a JSON backup from **Profile → Export backup** regularly. Browser data clearing or deleting the site's storage can erase local records. Re-deploying the same app to the same URL keeps the same storage origin.

## Important limitations

- This ZIP is a ready-to-host PWA package, not an already-published public website or Play Store app.
- GitHub Pages hosting is a one-time manual setup. After hosting, the home-screen installation is straightforward.
- A browser may label installation **Install app** or **Add to Home screen**, depending on Android/Chrome version.
