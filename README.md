# XavierDrive v1.2.0 + XD Assist 1.0.0 delivery

Temporary delivery repo. **Delete after confirming download.** The old XD Rig
app is retired — removed everywhere, forget it existed.

## 1. XavierDrive v1.2.0 (THE fix release)

- File: `xavierdrive1.2.0.apk` (5.6 MB) — installs over 1.1.8/1.1.9 in place
- sha256: `c305744152bb725ab8989930dfd774ec12d3e3262304be7648a5a79a04821fd8`

### What finally changed (the things actually asked for):

- **Bug report button crash — FIXED.** Since 1.1.8 it crashed the whole app.
  The screen is now crash-proofed: whatever happens, it opens and shows any
  error in red INSIDE the screen instead of dying. If anything is still
  wrong on a specific phone, the exact error text shows on screen —
  screenshot it and that text IS the diagnosis.
- **Latest log — the 3-option menu (exact spec):**
  1. **Enable logging / Disable logging** — state-aware (logging is ON by
     default)
  2. **latestlog.txt** — opens the log INSIDE the app, with a **Download
     button at the top** of the viewer
  3. **What is logging?** — full plain-language explanation (what, why,
     privacy: never leaves the phone except inside a bug report you send)

## 2. XD Assist 1.0.0 (the white permissions app — replaces the Rig)

- File: `xdassist-1.0.0.apk` (25 KB)
- sha256: `7c3a4a5449f4157f067c3f0be33ac25cf8d12c9182c73cf3485b799e6a859b56`
- A tiny white app: type your Termux bridge URL + secure key, test the
  connection, then tap **ENABLE SCREEN CONTROL** and switch XD Assist ON in
  Android's Accessibility settings. After that, the bridge (running in your
  Termux) can read the screen and tap/swipe/type/back/home on the phone —
  so the XavierDrive app can be tested and fixed remotely. Nothing works
  until YOU enable it, and it only talks to the URL you typed.

## Install

Download the APK(s) from this repo (click file → Download) → open on the
phone → allow "install unknown apps" if asked. Both are release-signed with
the school key.
