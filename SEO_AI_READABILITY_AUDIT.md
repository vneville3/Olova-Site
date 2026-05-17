# SEO and AI Readability Audit

## Files changed in the SEO/AI pass

- `index.html`
- `products.html`
- `trade.html`
- `design.html`
- `community.html`
- `contact.html`
- `stories.html`
- `projects.html`
- `sitemap.xml`
- `llms.txt`
- `SEO_AI_READABILITY_AUDIT.md`

## Current canonical strategy

Vaughan approved using `Products` as the public-facing label and `products.html` as the canonical product URL.

- `products.html` is the indexed canonical product page.
- `trade.html` is compatibility-only and redirects to `products.html`.
- `trade.html` has `noindex,follow` and a canonical link pointing to `https://olovatrading.ca/products.html`.
- Product/Offer JSON-LD uses `https://olovatrading.ca/products.html` as the URL and stable entity base.
- `sitemap.xml` lists `https://olovatrading.ca/products.html` and intentionally does not list `https://olovatrading.ca/trade.html`.
- Public navigation uses `Products` as the label.

This removes the previous silent ambiguity between product and trade language. Trade language may still appear contextually where it describes future import or supply work, but it is no longer the main public page label or canonical URL.

## Issues found

- `products.html` was previously a redirect to `trade.html` even though Vaughan now wants Products as the public-facing label.
- `trade.html` carried the full SPINE/product content and canonical Product/Offer JSON-LD.
- Main navigation on current public pages still linked to `trade.html` with the `Trade` label.
- `sitemap.xml` listed `trade.html` instead of the approved canonical `products.html` URL.
- `llms.txt` documented the old products-to-trade redirect.
- The earlier audit notes still described Trade as the current canonical strategy.

## Fixes made

- Rebuilt `products.html` as the real product page using the existing SPINE/product layout and conservative product content.
- Updated `products.html` metadata, Open Graph, Twitter tags, canonical link, nav active state, footer label, inquiry subject, and Product/Offer JSON-LD to use Products and `https://olovatrading.ca/products.html`.
- Replaced `trade.html` with a compatibility redirect to `products.html`, including `noindex,follow` and a canonical link to `products.html`.
- Updated public navigation links from `Trade` / `trade.html` to `Products` / `products.html` on root content pages.
- Updated the home page's product-lane metadata and obvious public labels from selective trade/trade lane to selective product/product lane.
- Updated `sitemap.xml` so the sitemap includes `products.html` and excludes `trade.html`.
- Updated `llms.txt` so AI/crawler-facing site notes describe Products as canonical and Trade as a compatibility redirect.
- Updated this audit to record the approved canonical decision and the resulting implementation.

## Validation notes

- `robots.txt` still points to `https://olovatrading.ca/sitemap.xml`.
- `sitemap.xml` matches the approved canonical strategy by listing `products.html` and not listing `trade.html`.
- Root content pages checked for H1 count: `index.html`, `products.html`, `trade.html`, `design.html`, `community.html`, `stories.html`, `projects.html`, `belong-centre.html`, `contact.html`, and `404.html` each have exactly one H1 after this pass.
- JSON-LD remains conservative: no product price, price currency, sizes, stock count, shipping terms, product condition, licensed architecture claims, engineering claims, or full design-build claims were added.
- Referenced root-page assets under `assets/` were checked against the repository asset listing during the SEO/AI-readability pass; no binary media was changed in this canonical update.
- No visual layout changes were made.
- Main body copy was not rewritten beyond necessary product-page label/URL alignment and compatibility redirect text.

## Recommended human decisions

- Decide how long to keep `trade.html` as a compatibility redirect. Keeping it is safest for old links; removing it later is optional.
- Decide whether any outside profiles, bios, or social links should be updated from Trade to Products once the live page is verified.
- Decide whether `belong-centre.html` should stay as an indexed standalone page or eventually canonicalize into `community.html`.
- Decide whether legacy nested Shopify-style paths should be redirected, noindexed, or left as historical compatibility paths.
- Add richer SPINE product details only if verified later: price, available sizes, exact inventory, shipping terms, or product condition.

## Remaining human decisions

- Vaughan still needs to decide the long-term fate of `trade.html` after old links have had time to settle.
- Vaughan still needs to provide or approve any factual SPINE commerce details before they are added to metadata, schema, or body copy.
- Vaughan still needs to decide whether Belong deserves a standalone indexed page long term or should fold fully into Community.