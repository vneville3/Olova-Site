# SEO and AI Readability Audit

## Files changed in the SEO/AI pass

- `products.html`
- `trade.html`
- `design.html`
- `community.html`
- `contact.html`
- `stories.html`
- `sitemap.xml`
- `llms.txt`
- `SEO_AI_READABILITY_AUDIT.md`

## Current canonical strategy

The current site is intentionally using `trade.html` as the canonical public page for the product/trade lane.

- `trade.html` is the indexed canonical page.
- `products.html` is a compatibility redirect to `trade.html`.
- `products.html` has a canonical link pointing to `https://olovatrading.ca/trade.html`.
- Product/Offer JSON-LD uses `https://olovatrading.ca/trade.html` as the URL and stable entity base.
- `sitemap.xml` lists `https://olovatrading.ca/trade.html` and intentionally does not list `https://olovatrading.ca/products.html`.

This is clean as long as Vaughan wants `Trade` to remain the public-facing label. If Vaughan decides that `Products` should be the public-facing language, the clean future move is a single coordinated switch: make `products.html` the canonical page, update nav/title/meta/schema/sitemap to `products.html`, and make `trade.html` redirect or noindex. Do not leave both pages indexable for the same SPINE/product content.

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
- Refined `llms.txt` to use more concrete language and to document the products-to-trade redirect.

## Validation notes

- Root content pages checked for H1 count: `index.html`, `design.html`, `community.html`, `stories.html`, `trade.html`, `projects.html`, `belong-centre.html`, `contact.html`, and `404.html` each have exactly one H1 after this pass.
- `products.html` now also has exactly one H1, but remains a redirect to `trade.html`.
- `sitemap.xml` matches the current canonical strategy by listing `trade.html` and not listing `products.html`.
- `robots.txt` points to `https://olovatrading.ca/sitemap.xml`.
- JSON-LD remains conservative: no product price, sizes, stock count, shipping terms, licensed architecture claims, engineering claims, or full design-build claims were added.
- Asset existence was checked against the repository `assets/` directory listing.
- No binary files were changed.
- No visual layout changes were made.
- No main body copy was rewritten beyond the redirect page fallback text, metadata/schema, `llms.txt`, and alt text.

## Recommended human decisions

- Confirm whether `Trade` should remain the public-facing label and canonical URL for the product lane.
- If `Products` is preferred publicly, approve a coordinated canonical switch from `trade.html` to `products.html` instead of running both.
- Decide whether `belong-centre.html` should stay as an indexed standalone page or eventually canonicalize into `community.html`.
- Decide whether legacy nested Shopify-style paths should be redirected, noindexed, or left as historical compatibility paths.
- Add richer SPINE product details only if verified later: price, available sizes, exact inventory, shipping terms, or product condition.

## Remaining human decisions

- Same as the recommended human decisions above; the technical crawl/readability structure is currently consistent, but those naming and legacy-path calls need Vaughan's judgment before further canonical changes.
