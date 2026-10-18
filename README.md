# XD Delivery

Temporary public delivery repo (law 10 — delete after owner confirms download).

## XavierDrive v1.2.1 (code 24) — 2026-10-18
- **Download**: `xavierdrive1.2.1.apk` (5,600,916 B, release-signed, sha256 `17a6a94d…`)
- **What's new**: the empty bug-report hub is FIXED. Root cause: the content frame was declared with the wrong view type since v1.1.8 — the hub silently rendered nothing every single time. Now it opens with all its cards, every render step is logged to latestlog.txt, and the error fallback can never fail silently again.
- Also on the update channel: the app itself offers this update (Settings → Check for updates).

## XD Assist 1.0.1 (code 2)
- **Download**: `xdassist-1.0.1.apk` (25,334 B, release-signed)
- **What's new**: `open` command now works for every app (Android 11+ package-visibility fix) and the Bridge URL field pre-fills the eternal worker proxy URL — a fresh install only needs the secure key.
- Setup: install, paste the key into the Secure key field (Bridge URL is pre-filled), tap SAVE & TEST, then enable the accessibility service. The worker URL never changes, no matter how often the phone's tunnel restarts.
