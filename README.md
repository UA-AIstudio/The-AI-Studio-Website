# AI+ Studio — Files & workshops

A responsive resource collection for AI+ Studio, with University of Arizona Libraries visual branding.

## Website preview

[Open the AI+ Studio website](https://ua-ai-studio-files.frostystoat7.chatgpt.site) — owner-only preview; sign-in is required. GitHub Pages has not been enabled for this private repository.

## What is included

- Featured Intro to Gemini Notebook workshop linking to its repository.
- File cards with view and download links for the workshop slides and poster.
- Link to the UA-AIstudio AI news board project.
- Intro to Claude AI marked as coming soon because its repository currently has no files.
- Search, resource-type filters, empty-result reset, and keyboard-accessible workshop topic tabs.
- Responsive layouts for mobile and desktop.

## Files and local preview

`index.html` contains the page and resource cards, `style.css` contains the styles, `app.js` provides search and interactive topics, and `assets/` contains the Libraries logo.

Open `index.html` in a browser or serve this directory using any static web server. No dependencies or build step are required. Google Fonts loads from the web, with system-font fallbacks available.

## Add a resource

Add an `article.file-card` in the `file-grid` in `index.html`. Set `data-kind` to `slides`, `images`, or `projects`; add lowercase title and description keywords in `data-search`; and update its visible title, description, and links. Update the total shown in the All resources button and initial result count. Search and filtering work automatically for matching cards when the page loads. For a new category, also add a filter button with the corresponding `data-filter` value.

Resource listings are curated in the HTML, not automatically synchronized from GitHub. Files remain in their original repositories.

## Branding

The logo is sourced from [University of Arizona Libraries](https://lib.arizona.edu/logo.svg). Branding is included as requested; visual identity alone does not imply institutional endorsement.
