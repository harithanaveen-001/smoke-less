# Smoke Less — Offline PWA

This is the personal offline mobile version of the smoking exposure calculator.

## Files
- index.html — calculator app
- manifest.json — installable-app configuration
- service-worker.js — offline caching
- icons/ — app icons

## Test on your computer
A PWA should be served through localhost/HTTPS rather than opened directly as file://.

From this folder, run one of these:
- Python: `python -m http.server 8000`
- Then open: `http://localhost:8000`

## Test on an Android phone on the same Wi-Fi
1. Start the local server on your computer.
2. Find the computer's local IPv4 address, e.g. 192.168.1.10.
3. On the phone open `http://192.168.1.10:8000`.
4. For actual PWA installation, use an HTTPS deployment. Localhost is suitable for development; a normal phone connection to a LAN IP may not satisfy installability/security requirements in every browser.

## Recommended next step
Deploy this folder to an HTTPS host, install it on the phone, then test it in airplane mode. The calculator itself does not require an internet connection after its app files have been cached.
