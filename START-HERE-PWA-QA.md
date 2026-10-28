# ADHD Daily Planner — PWA V1

This package adds a Progressive Web App shell to the existing ADHD Daily Planner without changing the planner's core UI/logic.

## Included
- `index.html` — PWA-enabled planner
- `manifest.webmanifest` — install/app metadata
- `sw.js` — offline app-shell caching
- `icons/` — 192px, 512px and Apple touch icon

## Important
A service worker/PWA installation requires the app to be served from HTTPS (or localhost during testing). Opening `index.html` directly with `file://` will still run the planner, but PWA installation/offline service-worker behavior will not activate.

## Recommended QA
1. Serve the folder over HTTPS or localhost.
2. Open the planner once online.
3. Install it from the browser's install/add-to-home-screen option.
4. Close and relaunch the installed app.
5. Turn off the network and verify the app shell still opens.
6. Verify existing local data, Brain Dump, Focus timer and last-screen persistence remain intact.
7. Test an update after changing the app version/cache name.
