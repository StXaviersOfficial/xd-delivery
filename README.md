# XavierDrive v1.1.10 + XD Assist 1.0.0 delivery

Temporary delivery repo. **Delete after confirming download.** The old XD Rig
app is retired — removed everywhere, forget it existed.

## 1. XavierDrive v1.1.10 (THE fix release)

- File: `xavierdrive1.1.10.apk` (5.6 MB) — installs over 1.1.8/1.1.9 in place
- sha256: `273fede094738ba27aed2ccba98e17579ae6f8e15b4b9f0f81e171b7bbd1a69f`
- Also on the live update channel: 1.1.8/1.1.9 users get the update banner on
  next app launch (worker serves 23/1.1.10, APK at
  https://stxaviers.pages.dev/apk/xavierdrive1.1.10.apk)

### Why 1.1.10 (not 1.2.0)

Your version law: +0.0.1 every release, so 1.1.9 → 1.1.10. The "1.2.0" name
was a mistake (and that slot on pages.dev is the tombstone of the old tainted
build — it stays a tombstone).

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

## 3. Termux (the other half of the Rig replacement)

Step-by-step command list:
https://github.com/StXaviersOfficial/stxaviers-android/blob/main/termux/SETUP.md
(two terminals: `python server.py` + `cloudflared tunnel --url
http://127.0.0.1:25570`, then paste the link + your XD_KEY passphrase into
XD Assist — or into the chat so the developer can drive the phone.)

## Install

Download the APK(s) from this repo (click file → Download) → open on the
phone → allow "install unknown apps" if asked. Both are release-signed with
the school key.
