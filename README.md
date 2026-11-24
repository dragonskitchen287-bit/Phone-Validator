# PixelProTech Phone Number Validator — PWA Package

Free, offline-capable mobile number validator for about 230 countries and territories. No server, no accounts, no limits.

Files (keep flat): `index.html`, `manifest.json`, `service-worker.js`, `icon-192.png`, `icon-512.png`, `README.md`.

## Use it
- **One number:** pick a country, type the number. Or start with `+` and a country code and the country is detected for you.
- **Many numbers:** paste one per line, click Validate all, then Copy valid numbers or Download CSV (E.164 format).

## Deploy (GitHub Pages)
Use a NEW repo (for example `Phone-Validator`) so it does not mix with other apps. Add file → Upload files → drag all 6 files into the root → Commit. Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save. Open `https://<username>.github.io/<repo>/`.

## What it checks
Country calling code, number length, and mobile prefix patterns for most countries. Countries without a known pattern are checked by length only and the result says so. It does not check whether a number is active, and +1 numbers cannot be told apart between the US and Canada.

## Editing
Bump `pixelprotech-phone-validator-v1` to `-v2` in `service-worker.js` whenever you change `index.html`.
