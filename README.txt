Plain Website Generator 2 (PWA package)
=======================================

App name:     Plain Website Generator 2
Version:      2.1
Cache:        v1
Author:       Plain
Display mode: standalone
Created with HTML2APP. Your HTML was kept as it was; only the tags a PWA needs were added.

FILES IN THIS FOLDER
--------------------
  index.html
  manifest.json
  sw.js
  offline.html
  icons/icon-192.png
  icons/icon-512.png
  icons/icon-maskable-512.png
  icons/apple-touch-icon.png
  README.txt

IMPORTANT: THIS FOLDER IS NOT AN APP YET
----------------------------------------
Making this folder does not install anything on your phone. A PWA must be hosted at an
https:// address first. Opening index.html straight from your files will not offer
install or offline mode. (http://localhost also works for testing on a computer.)

STEP 1: PUT IT ONLINE
---------------------
GitHub Pages
  1. Unzip the file on your computer. Inside you will see index.html and other files.
  2. Sign in at github.com and create a new public repository (for example "my-app").
  3. On the new repository page choose "uploading an existing file". Drag in everything from inside the unzipped folder (the files, not the folder itself), then commit.
  4. Open the repository Settings, then Pages. Under "Build and deployment" choose "Deploy from a branch", pick the main branch and the / (root) folder, and save.
  5. Wait a minute or two. Your address will be https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/

Netlify
  1. Sign in at app.netlify.com (a free account is fine).
  2. Choose "Add new site", then "Deploy manually" (drag and drop).
  3. Drop the ZIP onto the upload area. If Netlify asks for a folder, unzip first and drop the unzipped folder.
  4. Netlify gives your app an address like https://your-site.netlify.app. You can rename it in Site settings.

Cloudflare Pages
  1. Sign in at dash.cloudflare.com (a free account is fine).
  2. Go to Workers & Pages, choose Create, then Pages, then "Upload assets" (direct upload).
  3. Name your project, then upload the unzipped folder or the ZIP and select Deploy.
  4. Your address will be https://your-project.pages.dev

STEP 2: INSTALL IT ON ANDROID
-----------------------------
  1. Open your hosted https:// address in Chrome on your Android phone.
  2. Let the page load fully once so the app can save itself for offline use.
  3. Tap the browser menu (three dots).
  4. Select "Install app" or "Add to Home screen" and confirm.
  5. Open the new icon on your home screen. The app launches in standalone mode, without browser bars.

On iPhone: open the address in Safari, tap Share, then Add to Home Screen.

UPDATING YOUR APP
-----------------
Replace the files on your host with the new ones. Each build gets its own cache, and old
caches are removed automatically. Phones pick up the update the next time the app is opened
online (you may need to close and reopen it once).

THINGS TO KNOW
--------------
- Offline mode only covers files that were saved on the first visit. Content your tool
  loads from the internet (data, APIs, live services) will not be available offline.
- Your HTML uses these online resources, which may not work offline:
    https://fonts.googleapis.com/css2?family=Hanken+Grotesk:wght@400;500;600;700&display=swap
    https://api.unsplash.com/search/photos?per_page=12&orientation=landscape&content_filter=high&query=
- Some tools store data in the browser. That data belongs to the web address, so moving to
  a new address starts fresh.
- If something looks stale after an update, clear the site data in Chrome settings.
