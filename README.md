# Runner Nyeri — Android-installable PWA prototype

## What this is
A Progressive Web App (PWA) package based on Runner Nyeri V2. When hosted on HTTPS, Android Chrome can install it to the home screen and open it in a standalone app-like window. It also includes a basic service worker for caching the app shell.

## Files
- `index.html` — customer, runner, business and overview screens
- `manifest.webmanifest` — install metadata and icons
- `service-worker.js` — app-shell caching for repeat/offline loading
- `icons/` — launcher icons

## Important limitations
This is still a prototype. Data is stored locally in the browser/device. Customers and runners on different phones do not share jobs. No real authentication, backend, dispatch, or payment processing is included. Do not use it to store sensitive data.

## How to install on Android
1. Upload the contents of this folder to an HTTPS static host (for example, a free static hosting service). Upload the files and folders without changing their relative paths.
2. Open the published HTTPS URL in Google Chrome on Android.
3. Use Chrome's menu and choose **Install app** or **Add to Home screen** (wording can vary).
4. Launch Runner Nyeri from the new home-screen icon.

Opening `index.html` directly as a local file will let you test the UI, but it will not enable PWA installation or service-worker/offline behavior.

## Zero-cost next step
Host the files on a free static hosting tier. Before serving real customers, build a shared backend, user authentication, access controls, privacy notice, runner verification process and operational support. Review Kenyan legal and tax obligations before commercial launch.
