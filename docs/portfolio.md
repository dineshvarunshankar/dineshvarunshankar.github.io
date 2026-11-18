# Portfolio homepage

The homepage uses `_layouts/portfolio.liquid`, which inherits al-folio's default layout. The existing bio and portrait remain in `about.md`, news comes from `_news`, and contact/profile links use `_config.yml`.

Edit homepage sections in `_data/portfolio.yml`. Empty `entries` arrays hide their section and navigation link. Entries support title, authors (Markdown), meta, description (Markdown), category, featured, media, media_alt, and links (label/url objects). Use a leading slash for local paths and HTTPS for external resources. Link project pages and videos through the resource links.

The homepage CSS is scoped in `assets/css/portfolio.css`, including a lighter blue for dark mode. Other al-folio pages keep their current styling.

This is a layout draft: replace all sample entries before setting `preview: false` and publishing. The preview flag displays a notice; it does not prevent deployment or automatically hide sample entries.

Run `bundle exec jekyll serve` to review locally. Pull requests run a build-only check and upload a downloadable site artifact. The existing main-branch workflow continues to control public deployment. Check mobile/desktop layouts, dark mode, navigation, and resources before merging.
