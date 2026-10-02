# XavierDrive Delivery — v1.1.9 + XD Rig 1.0.0

Temporary delivery repo. **Delete after confirming download.**

## 1. XavierDrive v1.1.9 (school app update)

- File: `xavierdrive1.1.9.apk` (5.6 MB)
- versionName 1.1.9 · versionCode 22 · minSdk 24 · arm64-v8a + others
- Release-signed with the same upload key as every 1.x build — **installs directly
  over v1.1.8 as an update** (no uninstall needed).
- Changes: https-only OAuth completion signal, host-based Google sign-in page
  check (AuthActivity), single photo encode in ProfileSync, bug-endpoint dedupe
  (EP_BUGS), stale version strings fixed. Backend v2.5.1 is already live and
  serves this version.
- sha256: `cb6cb74cdef4d6de6c361ae055b49c40177850fc1dd5c1cd097b803f67a043a4`

## 2. XD Rig v1.0.0 (new app — on-phone terminal + backend)

- File: `xdrig-1.0.0.apk` (35.6 MB, arm64-v8a only, minSdk 24)
- Package `com.stxaviers.term` — a separate app from XavierDrive (installs
  side-by-side, own icon).
- What it is: a real local terminal (persistent `/system/bin/sh`, history
  up/down, Ctrl+C/Ctrl+D, ANSI colors, extra-keys row) + a "Set up backend"
  console that boots the REAL XavierDrive server.js on-phone via
  nodejs-mobile 18.20.4, with a cloudflared quick tunnel for public access and
  a copy-box popup for the BACKEND_KEY + tunnel URL.
- First screen is a password gate (rig/verify → /dev-login fallback, token
  RAM-only). Every error shows in-app in red — nothing silently fails.
- sha256: `b7fd2bd2b93cd82551202ac3bd46d802aa1dea7020589355e99158ba8632ae1d`

## Install

1. Download the APK(s) from this repo (click file → Download).
2. Open on the phone, allow "install unknown apps" for your browser/file
   manager if asked.
3. XD Rig 1.0.0 is a fresh app (no older version exists); XavierDrive 1.1.9
   updates 1.1.8 in place.
