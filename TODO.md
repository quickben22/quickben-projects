# TODO

## Website: add two more projects to the portfolio

Add project cards to `public/index.html` (Work section), following the existing "Prime or Not" card pattern. Consider updating the "More in the making" section since there are now three live apps.

### 1. Bitcoin Key Hunter
- Play Store: https://play.google.com/store/apps/details?id=com.quickben22.bitcoinlotto
- Display name: **Bitcoin Key Hunter**
- Category: Puzzle · Contains ads · PEGI 3 · 10K+ downloads · 3.0 rating
- Last updated: Nov 15, 2026
- Short blurb idea: "An app for searching lost Bitcoins. Also has a bitcoin riddle."
- Chips idea: `Android`, `Puzzle`, `Background search`

### 2. Bets Keeper
- Play Store: https://play.google.com/store/apps/details?id=com.companyname.AndroidTest3
- Display name: **Bets Keeper** (⚠️ the package id above currently resolves to Bets Keeper — verify this is the intended URL/package before publishing)
- Category: Sports · Contains ads · PEGI 3 · 1K+ downloads · 4.6 rating
- Last updated: Nov 12, 2026
- Short blurb idea: "Simple, no-nonsense betting record keeping app — just bet size and winning amount, everything else optional."
- Chips idea: `Android`, `Sports`, `Track results`

### After editing
- Update `public/styles.css` / `public/script.js` only if a third card needs layout changes.
- Check the site locally, then push to `master`.

## Blocked: GitHub Actions auto-deploy

- Deploy workflow now triggers on `master`, but the run fails with `Input required and not supplied: firebaseServiceAccount`.
- The repo has no Actions secrets configured.
- Fix: add repository secret `FIREBASE_SERVICE_ACCOUNT_QUICKBEN_PROJECTS` with the full Firebase service account JSON (Firebase Console → Project settings → Service accounts → Generate new private key), then re-run the failed workflow.
