# New Again — Gratitude Journal

A mobile-friendly, local-first gratitude journal inspired by the supplied New Again reference.

## Features
- Three daily gratitude entries, saved automatically in browser localStorage
- Repeat detection excludes the current entry itself and checks other saved entries only
- History includes today's entries as well as previous days
- Searchable collection, streaks, counts and a seven-day practice chart
- Repetition sensitivity setting
- JSON backup/restore and CSV is intentionally omitted in this redesign
- Installable/offline PWA shell
- No account, analytics, remote AI calls, or server-side journal storage

## Publish with GitHub Pages
Upload `index.html`, `manifest.webmanifest`, `sw.js`, and this README to the root of a GitHub repository. Then open Settings → Pages, choose Deploy from a branch, select `main` and `/ (root)`, and save.

## iPhone
Open the HTTPS Pages URL in Safari → Share → Add to Home Screen. Data is saved in that browser's local storage. It does not sync automatically with other devices. Export a JSON backup regularly.

## Storage note
Browser storage is local to the browser/device and can be cleared by the user or browser. Export backups regularly. The app cannot silently write into arbitrary hard-drive folders; exports are downloaded and saved where you choose.

## Repeat detection
The checker is a local heuristic, not a semantic AI model. It excludes the entry being edited and can warn about matching wording or selected related concepts. It may miss paraphrases or flag unrelated entries; the user can always keep a flagged moment.
