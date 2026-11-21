# Quickben — Independent Developer

Source for the static portfolio site deployed at <https://quickben-projects.web.app/>.

> **Note:** this repository is a reconstruction of the live site. The original source was not present on the local machine, so these files were recovered from the public deployment on 2026-11-21. They reproduce the currently deployed HTML, CSS and JavaScript.

## Files

- `public/index.html` — single-page portfolio (Work / About / Contact)
- `public/privacy.html` — privacy policy page
- `public/styles.css` — all styling, including responsive breakpoints
- `public/script.js` — footer year and mobile menu toggle
- `firebase.json` / `.firebaserc` — Firebase Hosting config targeting project `quickben-projects`

## Local preview

Serve the `public` folder with any static server, e.g.:

```powershell
cd public
npx serve .
```

Or Python:

```bash
cd public
python -m http.server 8080
```

Then open <http://localhost:8080/>.

## Deploy to Firebase Hosting

```bash
npm install -g firebase-tools
firebase login
firebase deploy --only hosting
```

The project ID in `.firebaserc` is `quickben-projects`. Deploying will overwrite the current live site, so preview locally first.
