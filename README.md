# LHZ Quiz: offline PWA

Files: index.html, sw.js, manifest.json, icons/, netlify.toml, .nojekyll

## 1. Host it (pick one, all free, all HTTPS)
**Netlify Drop (fastest):** open app.netlify.com/drop, drag this whole folder in. Done, you get a link.
**GitHub Pages:** new repo, upload every file in this folder (keep the icons/ folder), then Settings > Pages > Deploy from branch > main / root.

## 2. Install on phones (PWA)
Open the link ONCE while online (this caches the app), then:
- Android Chrome: menu > Install app
- iPhone Safari: Share > Add to Home Screen
After that it opens and runs with no internet. Results queue on the device and send automatically when data returns.

## 3. Make the APK
Easiest: go to pwabuilder.com, paste your hosted link, click Package for Stores > Android. Download the zip: it contains a signed .apk (share directly) and a .aab (Play Store). Keep the signing key file it generates; you need it for every future update.

## Updating later
Edit index.html, change VERSION in sw.js (e.g. lhz-quiz-v2), re-upload. Phones update on next online open. The APK needs no rebuild; it loads your hosted site.
