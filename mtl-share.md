# Sharing: mtl (pronounced "metal") — a local-first mood mix app

**Repo:** [nd28/mtl](https://github.com/nd28/mtl)
**Latest build:** [Download latest APK](https://github.com/nd28/mtl/releases/latest/download/app-debug.apk)
*(Points at the newest non-prerelease release. If it 404s, grab the newest build from the [releases page](https://github.com/nd28/mtl/releases).)*

## What it is

**mtl** is a local-first app for "mood mixes": playlists made of notes, articles, photos,
videos, audio sketches, saved links and small games, plus a cabinet of shelves and highlights.
Everything is stored on your device in IndexedDB — there is no backend and no account.

## Getting started (Android, first 5 minutes)

1. Download and install the APK from the link above, then open mtl. You land on **Today** with
   an empty state and a prompt to compose your first item. Nothing is uploaded anywhere.
2. Tap **Compose** (the round button with a plus icon in the bottom-right corner) → **Record**
   to capture a meeting (audio sketch) or a quiet moment (note + photo). Give it a short title
   and a vibe (mood tag) that matches how it feels.
3. Save it — it shows up on Today and in the Feed.
4. Go to **Mixes → New mix**, name it after the moment (e.g. "Peaceful morning"), and add the
   captures you just made.
5. Open the mix and press play to walk through everything you captured.
6. Later, open any item and leave a comment — it'll be there when you revisit.

## Why I'm sharing it

- It is a fully offline, no-account app — your data stays on your device.
- It is built to be shared into: from Instagram, YouTube, Pinterest etc. via the Android
  share sheet, or as a PWA share target.
- It shows how far a local-first, single-device app can go without a server.

## A day with mtl

- **Morning meeting** → record an audio sketch plus a quick note.
- **Quiet moment later** → capture thoughts/photos and tag the vibe.
- **Evening** → build a mix from the day's captures and replay it.

## What you can do

- **Today** (home screen) — a greeting, a "resume last mix" shortcut, and highlights of recent saves and shelves.
- **Feed** — stream of saves with type filters.
- **Save** — quick-save: paste a link, pick media, record (also the share-target landing page).
- **Mixes** — create playlists ("mixes") and get suggestions for a mood; play a mix.
- **Items** — per-type detail pages with reactions, comments (add your thoughts when you revisit a save), save and highlight.
- **Compose** — create and edit all item types.
- **Cabinet / shelves / highlights** — organize and pin what matters.
- **Games** — small built-in games.
- **Settings** — preferences and data management.

## Tips

- Share into mtl from Instagram, YouTube, Pinterest etc. via the Android share sheet.
- Use comments to leave thoughts on a save so future-you remembers why it mattered.
- Backups live in `Documents/mtl-backups/` on the device.
- To remove the app and its data, uninstall normally from Android settings.

## Backups

Auto-backups and exports go to `Documents/mtl-backups/` on the device.

## Installing the Android build

1. Download the APK from the release link above.
2. On your Android device, allow installing from your browser/file manager.
3. Open the APK and install.

## Technical details (optional)

- Built as a TanStack Start SPA, wrapped with Capacitor for Android, and also runnable in a browser as a PWA.

## Notes

- No network traffic beyond your own device; safe to use offline.
- If you hit issues, the project tracker is [`TRACKER.md`](https://github.com/nd28/mtl/blob/main/TRACKER.md).