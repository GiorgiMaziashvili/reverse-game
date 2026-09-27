# Reverse Audio

A mobile-friendly, pass-the-phone audio guessing game for 2–4 teams.

Record a phrase, play it backwards, and let the opposing team record an imitation and reverse it to guess the original. Choose round points, judge the answer, and rotate players automatically.

Game progress is stored in localStorage; recordings are stored in IndexedDB. The three-dot menu includes Quit Game and New Game. Starting a new game clears this game's saved data.

## Play locally

Run `python3 -m http.server 8765` in this folder, then open http://localhost:8765. Allow microphone access when prompted.

## GitHub Pages

In repository Settings → Pages, select **Deploy from a branch**, choose **main** and **/ (root)**, then save.

The published URL will be https://GiorgiMaziashvili.github.io/reverse-game/ . HTTPS enables microphone access on phones. Saved games belong to the browser and site address where they were created.

## Install on a phone

Publish all files in this folder, including `manifest.webmanifest`, `sw.js`, and `icons/`.

- iPhone/iPad: open the HTTPS site in Safari, select Share → Add to Home Screen, enable Open as Web App when shown, and tap Add.
- Android: open the HTTPS site in Chrome and select Install app or Add to Home screen → Install. The game's three-dot menu also offers installation help or the native install prompt when available.

Launch from the new home-screen icon to use the standalone app window without the browser address bar. The app shell is cached after the first online visit. Device installation and microphone permissions must be checked on an actual phone. New games always start with Team A; existing saved rounds remain intact.
