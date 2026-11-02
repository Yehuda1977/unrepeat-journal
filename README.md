# Unrepeat — local-first gratitude journal

A lightweight, mobile-friendly gratitude journal inspired by the idea of finding three new things to appreciate each day.

## Features
- Three daily entries, saved automatically in browser `localStorage`
- Repeat warnings using exact/substring matching plus a small local synonym/concept heuristic
- Daily history
- JSON backup and restore
- CSV export
- Installable PWA shell (Add to Home Screen / install where supported)
- No account, analytics, external AI calls, or server-side journal storage

## Important note about repeat detection
The app's repeat checker is deliberately local and privacy-preserving. It catches exact wording, close phrase overlap, and selected related concepts. It is **not** a true semantic AI model and can miss paraphrases or flag unrelated entries. A genuinely strong semantic checker would require bundling a local embedding model (larger download) or using a remote AI service (which would send journal text off-device).

## Publish with GitHub Pages
1. Create a new GitHub repository, for example `unrepeat-journal`.
2. Upload `index.html`, `manifest.webmanifest`, `sw.js`, and this README to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then Save.
6. Wait for the Pages URL to appear in Settings → Pages.

## Use on iPhone
1. Open the published HTTPS GitHub Pages URL in Safari.
2. Tap Share → Add to Home Screen.
3. Launch from the new Home Screen icon.

Safari stores the journal in that web app's browser storage on the iPhone. It does not automatically sync with your Mac or other browsers.

## Storage and backups
- Entries are saved in the browser on the device you use.
- Export JSON regularly. Keep the backup in Files, iCloud Drive, or a folder on your computer.
- Import a JSON backup on another device to transfer your journal.
- Clearing browser website data can erase the local journal. Export a backup first.
- The app cannot silently write to arbitrary folders on your hard drive. Export creates a downloadable file that you choose where to save.

## Local preview
Open `index.html` in a browser. For PWA/offline behavior, serve the folder over HTTPS or a local development server.
