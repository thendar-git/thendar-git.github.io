# thendar-git.github.io

Games by Thendar, served by GitHub Pages at https://thendar-git.github.io.

- `index.html`: the games page, one large tile per game.
- `word-jungle/`: Word Jungle's page, its images (`img/`) and its privacy policy (`privacy/`, linked from Play Console and from the app).
- `privacy/`: forwards to `/word-jungle/privacy/`, the policy's first address.
- `app-ads.txt`: AdMob's authorized-seller file for every game. It must stay at the site root.
- `assets/`: the shared stylesheet and site icons.

## Adding a game

1. Make a folder named after the game (e.g. `my-game/`) with its `index.html`, `img/` and `privacy/index.html`. Copying `word-jungle/` is the quickest start.
2. Add a tile for it in `index.html`: copy the Word Jungle `<li>` and change the link, images and text. The feature image is 1024×500.
3. If the game shows AdMob ads under a different publisher ID, add its line to `app-ads.txt`.

Plain HTML and CSS with no build step. Edit a file, push to `main`, and Pages republishes in about a minute.

Browsers keep `assets/style.css` for up to 10 minutes. After changing it, bump the `?v=` number in every page's stylesheet link so visitors get the new version at once.
