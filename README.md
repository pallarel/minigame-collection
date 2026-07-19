# Hardle

A dependency-free, single-page Hardle game. Progress, theme preference, completed-game history, win rate, and streaks are stored only in the player's browser with `localStorage`.

## Publish with GitHub Pages

1. Create a GitHub repository and push this folder to its `main` branch.
2. Open **Settings → Pages** in the repository.
3. Under **Build and deployment**, set **Source** to **GitHub Actions**.
4. Open the **Actions** tab and wait for **Deploy Hardle to GitHub Pages** to finish.

The deployment URL appears in the completed workflow and in **Settings → Pages**. Every later push to `main` automatically republishes the site.

## Run locally

Because the dictionaries are fetched over HTTPS, serve the folder instead of opening the HTML with a `file://` URL. For example:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.
