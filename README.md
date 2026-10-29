# Board Game Hub

A single-file, no-build web app with playable board games:

- Snakes & Ladders (randomized boards, modern and traditional themes)
- Puli Meka (Tigers & Goats)
- Ludo and Pachisi / Chausar (cowry throws)
- Chess (clocks, full screen, undo, King of the Hill, Three-check, six piece sets, eight boards, computer opponent)
- Sri Krishna: luxury wooden property-trading board

Dice games use a kinetic tray: drag and flick the dice to roll.

## Run locally
Open `index.html` in a browser.

## Host on GitHub Pages
1. Create a new repository on GitHub (for example `board-game-hub`).
2. Upload `index.html`, `.nojekyll` and `README.md` (Add file, then Upload files).
3. Go to Settings, then Pages. Under Build and deployment choose "Deploy from a branch", branch `main`, folder `/ (root)`, and Save.
4. After a minute the game is live at `https://<your-username>.github.io/board-game-hub/`.

## Add a new game
Inside `index.html`, call `Hub.register({id, name, icon, color, tagline, status:'ready', options:[...], mount(el, opts, api){...}})`. The menu card and setup screen are generated automatically.
