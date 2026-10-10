# Daily Tree

Hierarchical task manager PWA: Category → Project/Routine → Task → Subtask.

## Run locally
    cd daily-tree && python3 -m http.server 8080
Open http://localhost:8080 (service worker works on localhost).

## Install on Android
Host the folder on any HTTPS static host (GitHub Pages, Netlify, Cloudflare Pages),
open it in Chrome on the phone, then menu → Add to Home screen / Install app.
Works offline after the first load.

## Data
Stored in the browser (localStorage) on each device. Settings → Copy backup / Restore to move data.

## Badges
- number: days since anything inside was last done
- red: 7+ days, a scheduled routine day was missed, or a deadline passed
- ✓: something was done today
- -: nothing planned
- round check on a bar: finishes the task shown on that bar
