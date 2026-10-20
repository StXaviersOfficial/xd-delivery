# XD Delivery

Temporary public delivery repo (law 10 — delete after owner confirms download).

## XavierDrive v1.2.3 (code 26) — 2026-10-20
- **Download**: `xavierdrive1.2.3.apk` (5,600,916 B, release-signed, sha256 `f8bd4e03…aaeb`)
- **What's new**: smoother on low-end phones — the login/splash animated backgrounds stopped allocating hundreds of gradient objects per second (zero visual change), and a new crash-proof typed view-lookup helper means a layout/code mismatch can never silently blank a screen again (the v1.1.8 bug-report-hub class of bug, now structurally impossible in new code).
- Housekeeping in the same release: the Git repo is now app-source-only (XD Assist + Termux bridge moved to their own repo `xd-assist`; no more APK binaries committed), and `start-bridge.sh` no longer 404-overwrites itself on repo moves — **on the phone, re-download it once**: `curl -sfLO https://raw.githubusercontent.com/StXaviersOfficial/xd-assist/main/termux/start-bridge.sh && bash start-bridge.sh`.
- Also on the update channel: the app itself offers this update (sha256-pinned) — Settings → Check for updates.

## XavierDrive v1.2.2 (code 25) — 2026-10-19
- **Download**: `xavierdrive1.2.2.apk` (5,600,916 B, release-signed, sha256 `4fb08c43…da7ac`)
- **What's new**: dashboard "Latest notice" now aggregates every class folder (it used to say "No notices yet" whenever any class had notices), and **updates are integrity-checked** — the APK's SHA-256 is verified before anything is offered for install. Plus the S25 full-sweep hardening behind the scenes (honest bridge errors, cookie-crash fix, tighter role matching).
- Also on the update channel: the app itself offers this update (sha256-pinned) — Settings → Check for updates.

## XavierDrive v1.2.1 (code 24) — 2026-10-18
- **Download**: `xavierdrive1.2.1.apk` (5,600,916 B, release-signed, sha256 `17a6a94d…`)
- **What's new**: the empty bug-report hub is FIXED. Root cause: the content frame was declared with the wrong view type since v1.1.8 — the hub silently rendered nothing every single time. Now it opens with all its cards, every render step is logged to latestlog.txt, and the error fallback can never fail silently again.
- Also on the update channel: the app itself offers this update (Settings → Check for updates).

## XD Assist 1.0.1 (code 2)
- **Download**: `xdassist-1.0.1.apk` (25,334 B, release-signed)
- **What's new**: `open` command now works for every app (Android 11+ package-visibility fix) and the Bridge URL field pre-fills the eternal worker proxy URL — a fresh install only needs the secure key.
- Setup: install, paste the key into the Secure key field (Bridge URL is pre-filled), tap SAVE & TEST, then enable the accessibility service. The worker URL never changes, no matter how often the phone's tunnel restarts.
