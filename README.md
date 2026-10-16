# AI+ Studio files

AI+ Studio Files is a simple website for browsing the public repositories, folders, and files in [UA-AIstudio](https://github.com/UA-AIstudio). It brings workshop materials, presentations, and project resources into one searchable directory. Visitors can expand folders and open files directly on GitHub.

## Links

- **Live website:** [AI+ Studio Files on GitHub Pages](https://ua-aistudio.github.io/The-AI-Studio-Website/)
- **Website source code:** [UA-AIstudio/The-AI-Studio-Website](https://github.com/UA-AIstudio/The-AI-Studio-Website)
- **GitHub organization:** [UA-AIstudio](https://github.com/UA-AIstudio)

The website is publicly accessible without signing in. Use **Refresh from GitHub** to fetch the latest public files and folders.

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
