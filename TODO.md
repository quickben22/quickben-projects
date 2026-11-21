# TODO

## Done: website lists all three projects

`public/index.html` now has cards for Prime or Not, Bitcoin Key Hunter and Bets Keeper, with matching visual variants in `public/styles.css`. The footer Google Play link points to the developer page.

## Blocked: GitHub Actions auto-deploy

- Deploy workflow now triggers on `master`, but the run fails with `Input required and not supplied: firebaseServiceAccount`.
- The repo has no Actions secrets configured.
- Fix: add repository secret `FIREBASE_SERVICE_ACCOUNT_QUICKBEN_PROJECTS` with the full Firebase service account JSON (Firebase Console → Project settings → Service accounts → Generate new private key), then re-run the failed workflow.
