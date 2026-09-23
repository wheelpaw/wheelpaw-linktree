# wheelpaw.de — Linktree

A minimal "link in bio" page for **wheelpaw.de**, built as a single static HTML file and hosted on GitHub Pages.

**Live site:** [https://wheelpaw.de](https://wheelpaw.de)

## Features

- Single-file, dependency-free static page (no build step)
- Dark theme with a paw-print avatar and inline SVG icons
- Links to Instagram and Bluesky

## Project Structure

```
.
├── index.html   # The entire page (markup + styles)
├── index.js     # Placeholder dev script
└── package.json
```

## Getting Started

### Local preview

Since `index.html` is fully static, you can simply open it in a browser, or serve it with any static file server, e.g.:

```bash
npx serve .
```

## Customization

All content lives in `index.html`:

- **Name / title** — edit the `<h1 class="name">` element
- **Links** — add or edit entries inside the `<nav class="links">` block; each link is an `<a class="link">` with an inline SVG icon and a label
- **Avatar icon** — replace the SVG inside `.avatar`
- **Colors** — adjust the CSS custom values at the top of the `<style>` block (background `#1a1a1a`, accent `#ffffff`)

## Deployment

This site is deployed via [GitHub Pages](https://pages.github.com/). Push to the repository's default branch (or configured Pages branch/folder) and GitHub will publish `index.html` automatically. The custom domain is configured via the `CNAME` file (containing `wheelpaw.de`) in the repository root; the corresponding DNS records are set up as described in the [GitHub Pages custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

## License

Private project — no license specified.
