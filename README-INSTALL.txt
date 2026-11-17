PUBLIC CAB — PWA HOSTING PACKAGE

This is a Progressive Web App (PWA), not an APK. Do not rename index.html or try to install it as an APK.

UPLOAD
1. Open the GitHub repository used by your Public Cab website.
2. Upload/replace the contents of this ZIP into the SAME folder that currently contains the live index.html.
3. Keep this exact structure:
   index.html
   manifest.webmanifest
   sw.js
   icons/icon-192.png
   icons/icon-512.png
4. Commit/publish and wait for GitHub Pages deployment.
5. Open the HTTPS website in Chrome and confirm the page loads.

INSTALL ON ANDROID
1. Open the website in Google Chrome (not WhatsApp's in-app browser).
2. Open Chrome ⋮ menu.
3. Choose "Install app" (or "Add to Home screen" if that is what Chrome offers).
4. Confirm Install.
5. Launch Public Cab from the phone's app drawer/home screen.

IMPORTANT
- This package is a PWA. It does not create or contain base.apk.
- The Android message "There was a problem while parsing the package" appears when Android is asked to install an APK; it is not the normal Chrome PWA install flow.
- Manifest and service worker are scoped to the current folder, supporting GitHub Pages project URLs such as https://username.github.io/repository/.
- Keep the existing website folder path unchanged.
- Admin logo changes update the running website UI. To change the launcher icon for future installs, replace icons/icon-192.png and icons/icon-512.png with correctly sized PNGs and redeploy; an already-installed app may retain its previous icon until refreshed/reinstalled.
- GPS and other browser features require HTTPS and user permission.
- Firebase/database access and live payment flows still depend on the existing Firebase configuration and security rules.
