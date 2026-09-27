# Reverse Audio

A mobile-friendly, pass-the-phone audio guessing game for 2–4 teams.

Record a phrase, play it backwards, and let the opposing team record an imitation and reverse it to guess the original. Choose round points, judge the answer, and rotate players automatically.

Game progress is stored in localStorage; recordings are stored in IndexedDB. The three-dot menu includes Quit Game and New Game. Starting a new game clears this game's saved data.

## Play locally

Run `python3 -m http.server 8765` in this folder, then open http://localhost:8765. Allow microphone access when prompted.

## GitHub Pages

In repository Settings → Pages, select **Deploy from a branch**, choose **main** and **/ (root)**, then save.

The published URL will be https://GiorgiMaziashvili.github.io/reverse-game/ . HTTPS enables microphone access on phones. Saved games belong to the browser and site address where they were created.
