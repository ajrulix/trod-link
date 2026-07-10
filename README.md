# Trod smart links

Serves invite links for the Trod app (https://gettrod.com).

- `index.html` — the smart-link page: tries the app deep link, falls back to Google Play.
- `404.html` — copy of index.html so path-style links (`/add/<handle>`, `/c/<code>`) work on GitHub Pages.
- `.well-known/assetlinks.json` — Android App Links verification. Currently holds the DEBUG
  signing fingerprint (dev-client builds). Add the RELEASE keystore fingerprint (and the
  Play App Signing fingerprint at launch) before shipping signed builds.
