# PsychDesk — deployment staging

This branch is reserved for PsychDesk. The existing `main` branch is untouched.

## Intended architecture
- GitHub Pages for the static frontend
- Firebase project `psystudy-e4854` for Google Authentication and Firestore account sync
- Google Drive for optional manual backups
- Gemini for study assistance after secure API setup

## Before enabling the site
1. Upload the complete contents of the PsychDesk 3.0 website ZIP at the repository root, including `index.html`, `app.js`, `cloud.js`, `firebase-sync.js`, `firebase-config.js`, `style.css`, `manifest.webmanifest`, `sw.js` and `icons/`.
2. Deploy the supplied account-scoped Firestore rules in Firebase.
3. Enable Google as a sign-in provider in Firebase Authentication, and authorize the GitHub Pages domain `sid964.github.io`.
4. Enable GitHub Pages for the deployment branch, or create a standalone `psychdesk` repository for a cleaner site URL.

**Privacy:** Never commit actual Gemini API keys, Drive access tokens, service account secrets, personal notes or study exports to a public GitHub repository.

The code has not yet been deployed or tested against the live Firebase project.
