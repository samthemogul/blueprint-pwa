# Transformation Blueprint

Installable iPhone web app (PWA) for a 26-week fat-loss and training plan: calorie and macro calculator, Nigerian 7-day meal plan, home and gym programmes, and a weight tracker. Location-aware: add stays (London or Lagos, with or without gym access) in Plan, and meals, activity tips, sessions and calories follow where you are on each date. Data stays on the device; export a backup from Plan → Your data.

## Deploy
Static site, no build step. On Vercel: framework preset **Other**, no build command, output directory `./`. `vercel.json` sets cache headers for the service worker and manifest.

## Updating
Bump `VERSION` in `sw.js` on every change so installed copies pick up the new files.
