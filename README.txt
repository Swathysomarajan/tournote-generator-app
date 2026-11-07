TOUR NOTE — PWA VERSION (based on your uploaded V11)

This package keeps your uploaded V11 Tour Note Generator as the current app and adds:
- Installable PWA manifest
- Tour Note app icon
- Service worker for caching the app shell
- Home-screen installation support on compatible mobile browsers

Deploy:
1. Extract this ZIP.
2. Upload the CONTENTS of the `tour_note_generator` folder to the root of your existing GitHub Pages or Netlify site, preserving the `icons` folder.
3. Replace the old index.html and add manifest.webmanifest, service-worker.js, and icons/tour-note.svg.
4. Open the site over HTTPS.
5. On Android Chrome: browser menu > Install app (or Add to Home screen).

Notes:
- This PWA caches the app shell so the page can reopen offline after the first successful visit.
- The PDF library is loaded from cdnjs in the existing V11 code. PDF generation therefore still requires internet unless that library is separately bundled locally.
- For GitHub Pages, keep all these files at the same site root and do not upload the ZIP itself.

Version 12 change: The installed app display orientation is set to portrait. The generated Tour Note PDF remains A4 landscape.
