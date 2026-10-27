BARTHOLOMEW 3D — INSTALLABLE WEB APP

Files in this folder:
- index.html: the 3D robot training app
- manifest.json: install name, app display mode, and icon definitions
- sw.js: service worker for caching the app shell
- icon.svg, icon-192.png, icon-512.png: app icons

PUBLISH TO YOUR EXISTING GITHUB REPOSITORY
1. Open your repository: https://github.com/admiralspace1214-commits/bartholomew
2. Create a new folder named bartholomew-3d (or upload these files into a new folder with that name).
3. Put ALL files from this package inside that folder. The structure should be:
   bartholomew-3d/index.html
   bartholomew-3d/manifest.json
   bartholomew-3d/sw.js
   bartholomew-3d/icon.svg
   bartholomew-3d/icon-192.png
   bartholomew-3d/icon-512.png
4. Commit the files to the main branch and wait for GitHub Pages to update.
5. Open this URL in Chrome on Android:
   https://admiralspace1214-commits.github.io/bartholomew/bartholomew-3d/
6. In Chrome, open the three-dot menu and choose "Install app" or "Add to Home screen" (the wording can vary).

NOTES
- This package does not replace your original index.html or existing Bartholomew app.
- The app icon/name should appear when installed as a PWA. Android/Chrome decides the final install UI.
- The app shell can be cached, but the Three.js 3D library is loaded from jsDelivr, so the 3D view still needs internet unless that library is separately bundled/cached.
- Training currently resets on refresh. Persistent brain-saving is a future update.
