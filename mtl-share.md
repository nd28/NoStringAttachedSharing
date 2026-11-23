# Sharing: mtl (pronounced "metal") — a local-first mood mix app

**Repo:** [nd28/mtl](https://github.com/nd28/mtl)
**Latest build:** [Download latest APK](https://github.com/nd28/mtl/releases/latest/download/app-debug.apk)
*(Points at the newest non-prerelease release. If it 404s, grab the newest build from the [releases page](https://github.com/nd28/mtl/releases).)*

## What it is

**mtl** is a local-first app for "mood mixes": playlists made of notes, articles, photos,
videos, audio sketches, saved links and small games, plus a cabinet of shelves and highlights.
Everything is stored on your device in IndexedDB — there is no backend and no account.

## Why I'm sharing it

- It is a fully offline, no-account app — your data stays on your device.
- It is built to be shared into: from Instagram, YouTube, Pinterest etc. via the Android
  share sheet, or as a PWA share target.
- It shows how far a local-first, single-device app can go without a server.

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