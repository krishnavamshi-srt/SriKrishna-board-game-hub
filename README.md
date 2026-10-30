# Board Game Hub

One HTML file, no build step, eleven games:

| Game | Modes |
|---|---|
| Snakes & Ladders | single device, online room (2-4), randomized boards, two themes |
| Puli Meka | vs computer, single device, online room |
| Ludo, Pachisi / Chausar | single device, vs computer, online room (2-4), kinetic dice and cowries |
| Chess | vs computer (3 levels), single device, online room, clocks, 3 variants, 8 piece sets, 10 boards |
| Sri Krishna (property trading) | single device, online room (2-4), 64 selectable tokens |
| Guess Who? | vs computer, online room, 9 editions, fresh roster every game |
| Jigsaw Puzzle | 12 to 500 real pieces, built-in scenes or your own picture, online co-op |
| Tank's 1918 | 72 levels, 2-player co-op, custom map editor |
| Bubble Struggle 3 | 1-2 players on one screen |
| Skywire 2 | single player |

Every game has a Full screen button.

## Run locally
Open `index.html` in a browser.

## Host on GitHub Pages
1. Create a repository (for example `board-game-hub`).
2. Upload `index.html`, `.nojekyll` and `README.md`.
3. Settings, Pages: deploy from branch `main`, folder `/ (root)`.
4. Play at `https://<your-username>.github.io/board-game-hub/`.

## Online rooms
Create a room in any game marked Online room, share the 5-letter code or link, and friends join from any device.
Internet mode uses PeerJS (loaded from jsDelivr, public broker), so it needs internet access.
"Same device (tabs)" mode works offline between browser tabs of the same browser.
Action games (Tank's 1918, Bubble Struggle, Skywire) are local-only.

## Add a game
`Hub.register({id, name, icon, color, tagline, status:'ready', feat:['s','h','o'], online:{min,max}, options:[...], mount(el, opts, api){...}})`
