# Portfolio homepage

The homepage adapts [Jon Barron's source template](https://github.com/jonbarron/jonbarron.github.io) directly. His README permits personal reuse.

- HTML: `_layouts/portfolio.liquid`, based on upstream `index.html` (blob `f6c9a08c91e5c8931ee8f10642ccb1c8e250f45f`).
- CSS: `assets/css/barron.css`, copied from upstream `stylesheet.css` (blob `c3abbcb6c1680f1da3a7dfb1f67fd55f006cdf7c`). The added CSS makes section headings bold purple (`#6f42c1`), widens the page to a maximum of 1200px, makes the name bold, and crops the portrait to a true circle capped at 280px with a 20% zoom inside the circle. The original mobile layout is retained.
- The homepage is a standalone document. It does not inherit al-folio's navigation, styles, or scripts. Existing interior pages retain their theme.

Edit the bio and portrait in `about.md`, links in `_config.yml`, news in `_news`, and sections in `_data/portfolio.yml`. Section entries support title, authors (Markdown), meta, description (Markdown), media, media_alt, and links (label/url). Sections can also have a plain-text description. Empty sections are hidden.

Entries with images use the template's original thumbnail-and-text rows; entries without images use its existing section spacing. No placeholder images are generated. Sample entries are explicitly marked as placeholders and should be replaced with real details.

Run `bundle exec jekyll serve` locally. Pull requests run the existing Jekyll build and upload a site artifact; merging triggers the existing deployment workflow.
