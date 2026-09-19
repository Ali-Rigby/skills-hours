# Skill Hours

A one-page time tracker for practice skills (Python, Stats, Matlab, EEG, MRI — editable in the app).
Live timer, manual logging, daily/weekly goals, streaks, weekly bars and a daily-hours trend.
No build step, no backend: everything is in `index.html`, and your log is stored in the browser.

## Publish on GitHub Pages

1. Push this folder to a GitHub repository (e.g. `skill-hours`).
2. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
3. After a minute the app is live at `https://<your-username>.github.io/skill-hours/`.

## Add it to your phone like an app

- **iPhone (Safari):** open the URL → Share button → **Add to Home Screen**.
- **Android (Chrome):** open the URL → ⋮ menu → **Add to Home screen** / **Install app**.

It opens full-screen, works offline, and keeps its own data.

## Updating

Edit `index.html`, then bump `CACHE` in `sw.js` (v1 → v2 …) so installed phones fetch the new version, commit and push.
GitHub Pages redeploys automatically. The installed app picks up the change the next time it's opened twice (once to fetch, once to show).

## Backing up your data

Your log lives in that browser's storage (the home-screen app and the Safari tab are separate stores).
Use **Edit skills → Export JSON** now and then; **Import JSON** merges a backup into any device.
