# Paper Boat: River Journey — app homepage

Static app homepage, privacy policy, support page, and AdMob app-ads.txt, following the WordZoo site structure. No build tools, dependencies, tracking scripts, or external fonts are required.

## Preview

Run `python3 -m http.server 8080` in this folder, then open http://localhost:8080.

## GitHub Pages

Publish this repository using GitHub Pages (Settings → Pages → Deploy from a branch → main → / root). The expected URL is https://weidinger-c.github.io/Paper-Boat-River-Journey-App/ once Pages is enabled and these files are pushed. No deployment has been performed as part of creating the files.

- Marketing URL: site root
- Support URL: support.html
- Privacy URL: privacy.html

The App Store listing URL is not yet configured. Once the app's public listing is known, add its real link to the homepage; there is deliberately no placeholder download button.

## Advertising verification

app-ads.txt uses the supplied AdMob publisher ID. AdMob looks for this file at the root of the developer website domain. A GitHub Pages project path alone may not satisfy that lookup: also serve this same file at https://weidinger-c.github.io/app-ads.txt (via the user-site repository), or use a custom domain with this file at its root. Configure the published developer website in App Store Connect and verify its crawl status in AdMob.

## Assets and content

icon.png and assets/river.webp reuse the game's own artwork. assets/puzzle.webp is an actual English gameplay screenshot. Images are local and optimized. Privacy and support text are based on the current app implementation, including locally saved progress, Google AdMob/UMP, and the one-time ad-free purchase with unlimited hints. Recheck these pages when app behavior or SDK data practices change.

## Verification

All three pages were checked in Chromium at 320, 390, 768, and 1440 pixels: no horizontal overflow, failed assets, HTTP errors, or browser script errors. Navigation, the journey anchor, native FAQ expansion, and reduced-motion behavior passed. Desktop and phone screenshots were visually reviewed.
