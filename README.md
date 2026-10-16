# AI+ Studio files

A simple directory of public repositories, folders, and files in [UA-AIstudio](https://github.com/UA-AIstudio).

[Open the live website](https://ua-aistudio.github.io/The-AI-Studio-Website/) — hosted on GitHub Pages, publicly accessible without signing in.

## Features

- One directory list with expandable repositories and folders.
- Search across file paths and names, including collapsed folders.
- File links open the original file on GitHub.
- Refresh from GitHub fetches current public repositories and their file trees without credentials.
- A saved snapshot provides a fallback if GitHub is unavailable or rate limits requests.

Only public repositories are listed. Empty repositories display “No files yet.” Private repositories are never fetched by the browser. No sign-in tokens are embedded in the site.

## Run locally

Open `index.html` in a browser, or use any static web server. No installation or build is required.

`index.html` contains the layout, `style.css` contains the styling, and `app.js` renders the directory and handles search and refresh. `resources.json` is the saved public directory snapshot; `resources.js` exposes that snapshot as `window.STUDIO_REPOS` so it also works when opened locally. Refresh updates the current browser session without writing back to the repository.

The saved snapshot was generated on October 16, 2026. To update it permanently, regenerate `resources.json` from GitHub’s public repository and tree APIs, then update `resources.js` with `window.STUDIO_REPOS = <JSON>;`.

The University Libraries logo in `assets/` is sourced from https://lib.arizona.edu/logo.svg. The requested visual branding does not imply institutional endorsement.
