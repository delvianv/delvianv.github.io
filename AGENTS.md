# AGENTS.md

## Project overview
- Static personal portfolio site (no build system, package manager, or test/lint tooling in repo).
- Core content lives in `index.html`; assets live in `images/`; `README.md` is separate profile copy (not rendered by the site).

## Working in this repo
- Prefer editing `index.html` directly; it contains page structure, inline `<style>`, inline SVG icon symbols, and page content in one file.
- The site uses Bootstrap 5.3.6 via CDN `<link>` tags in `index.html` (with SRI/crossorigin attributes). Keep external asset references and metadata tags consistent when changing the page.
- Use relative/local paths for site assets (e.g. `images/...`) when adding or updating portfolio images.

## Verification
- No automated checks are configured. Verify changes by opening `index.html` in a browser.
- For a quick local preview server when needed: `python3 -m http.server` from the repo root, then open the reported localhost URL.

## Repo quirks
- Keep image filenames/paths aligned with references in `index.html` and social/preview metadata if those assets change.
