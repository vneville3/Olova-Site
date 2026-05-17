# SEO and AI Readability Audit

## Files changed

- `products.html`
- `trade.html`
- `design.html`
- `community.html`
- `contact.html`
- `stories.html`
- `sitemap.xml`
- `llms.txt`
- `SEO_AI_READABILITY_AUDIT.md`

## Issues found

- `llms.txt` did not exist.
- `sitemap.xml` was stale: it listed `products.html`, which redirects to `trade.html`, and did not list `stories.html`, `trade.html`, or `projects.html`.
- `products.html` was a redirect page with no H1.
- Structured data was already present on `index.html`, but missing from the other requested pages.
- A small number of image alt attributes were technically present but too generic to be useful.
- Root-page internal links resolved to existing root pages, anchors, mail links, or the YouTube embed.
- Referenced root-page assets under `assets/` were found in the repository asset listing.

## Fixes made

- Kept the existing `robots.txt` because it already allows crawling and points to the sitemap.
- Updated `sitemap.xml` to list the canonical root pages: home, design, community, stories, trade, projects, Belong Centre, and contact.
- Added `llms.txt` with a concise factual summary of OLOVA and key pages.
- Added conservative JSON-LD structured data:
  - `products.html`: `Offer` with SPINE as `itemOffered`, no price, size, or stock count invented.
  - `trade.html`: matching conservative SPINE `Offer` for the canonical trade page.
  - `design.html`: `Service` for skater-led concept design, visualization, review, and early-stage direction without architecture or engineering claims.
  - `community.html`: `WebPage` about Belong Youth Centre and community-linked skate/youth-space support.
  - `contact.html`: `ContactPage` with the public inquiry email.
- Preserved the existing `Organization` and `WebSite` JSON-LD on `index.html`.
- Added one H1 to `products.html` while preserving the redirect behavior.
- Improved only obvious weak alt text on SPINE and Stories images.

## Validation notes

- Root content pages checked for H1 count: `index.html`, `design.html`, `community.html`, `stories.html`, `trade.html`, `projects.html`, `belong-centre.html`, `contact.html`, and `404.html` each have exactly one H1 after this pass.
- `products.html` now also has exactly one H1, but remains a redirect to `trade.html`.
- Asset existence was checked against the repository `assets/` directory listing.
- No binary files were changed.
- No visual layout changes were made.
- No main body copy was rewritten beyond the redirect page fallback text and alt text.

## Remaining human decisions

- Decide whether `belong-centre.html` should stay as an indexed standalone page or eventually canonicalize into `community.html`.
- Decide whether legacy nested Shopify-style paths should be redirected, noindexed, or left as historical compatibility paths.
- Decide whether `products.html` should remain as a redirect or be removed from public navigation permanently in favor of `trade.html`.
- Add richer product details only if verified later: price, available sizes, exact inventory, shipping terms, or product condition.
