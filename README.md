# Level 70 mission chains

Interactive mission chains (level 60 and up) for two level 70 rewards:

- `goliath_tank_chain.html` - The Goliath Tank
- `spiderwasp_queen_chain.html` - Spiderwasp Queen (ends with the "Infiltration" mission that defeats the Queen)

Each page lists every mission in order, what has to be built and how long it takes. Pick the missions you are on and
everything before them drops out of the list and the item totals. The pages are single self-contained files (the only
outside request is the Google Fonts stylesheet). `images/` holds portrait and landscape pictures of each chain.

## GitHub Pages

The site is plain static files, so no build step is needed:

1. Push this folder to a GitHub repository.
2. In the repository, open Settings > Pages, set Source to "Deploy from a branch", pick the `main` branch and the
   `/ (root)` folder, and save.
3. After a minute the site is at `https://<user>.github.io/<repository>/` (`index.html` is the landing page).

`.nojekyll` tells Pages to serve the files as they are. All links are relative, so the site also works from a
repository subpath or when the folder is opened locally.

The pages are generated from game data; to update them, replace the two `.html` files and the pictures in `images/`.
