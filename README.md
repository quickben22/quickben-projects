# Quickben portfolio

Plain HTML, CSS and JavaScript portfolio with a responsive modern design.

## Before publishing
- Replace `public/app-ads.txt` with the exact seller authorization line shown in your AdMob account.
- Review `public/privacy.html` and make it accurate for your actual app, AdMob SDK, consent flow and data practices. Do not publish the draft unchanged.
- Check the public contact email and update it if needed.

## Deploy to Firebase Hosting
Install Node.js, then run from this folder:

```bash
npm install -g firebase-tools
firebase login
firebase projects:list
firebase use --add
firebase deploy --only hosting
```

Select your Firebase project when prompted. Test `/`, `/privacy.html` and `/app-ads.txt` on the resulting `PROJECT_ID.web.app` address.
