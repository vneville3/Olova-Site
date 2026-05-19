# OLOVA AI Readability Scorecard

Backend-only review of the current OLOVA AI/search-readable layer.

No HTML files were edited for this scorecard. No visible copy was changed. No binary assets were touched.

## Current score

Overall AI/search readability: **8.5 / 10**

This is strong for the current stage. The remaining gap is not basic SEO plumbing. The remaining gap is structured proof and page-level entity clarity.

## What is already working

### Crawler basics

- `robots.txt` allows crawling.
- `robots.txt` points to `https://olovatrading.ca/sitemap.xml`.
- `sitemap.xml` lists the current canonical public pages.
- `trade.html` is correctly excluded from the sitemap because it is compatibility-only.

Score: **9.5 / 10**

### Canonical clarity

- Public product label is currently `Products`.
- Canonical product page is `products.html`.
- `trade.html` redirects to `products.html`.
- `trade.html` is marked `noindex,follow`.
- `llms.txt` documents the Products / Trade relationship clearly.

Score: **9 / 10**

### AI-readable summary

`llms.txt` gives a clear compressed explanation of the site:

- OLOVA is skater-owned.
- OLOVA is based in the Tri-Cities, British Columbia.
- OLOVA is design- and community-led.
- Product is secondary.
- OLOVA does not claim to be an architecture firm, engineering firm, or full design-build skatepark company.

Score: **9 / 10**

### Metadata and schema

Strongest schema coverage currently appears on:

- Home: Organization / WebSite
- Products: Offer / Product
- Design: Service
- Community: WebPage
- Contact: ContactPage

Lighter or missing schema coverage appears likely on:

- Stories
- Projects
- Belong Centre

Score: **7.5 / 10**

### Copy protection

The separate writing layer is now protected by:

- `OLOVA_SITE_CURRENT_RULES.md`
- `OLOVA_SITE_HANDOFF.md`
- `VISIBLE_COPY_CHANGE_AUDIT.md`

This matters because AI-readability work should not rewrite Vaughan's refined visible copy.

Score: **9 / 10**

## Main remaining gaps

### 1. Schema is uneven

Some pages have strong JSON-LD. Others rely mostly on HTML metadata and visible content. That is not fatal, but a future backend-only schema validation report would help.

### 2. Project proof is not consistently structured

Projects would eventually benefit from consistent facts such as:

- project name
- location
- status
- Vaughan's role
- concept vs built vs archive
- media type
- claim limits

This should be handled as a review-first visible add-on if it appears on public pages.

### 3. Belong needs clearer entity handling later

`community.html` and `belong-centre.html` both mention Belong. That can be fine, but the relationship should eventually be made clearer:

- `community.html` = broader community lane
- `belong-centre.html` = dedicated Belong proof/entity page

Do not change visible Belong copy during SEO work.

### 4. Stories and Projects can become stronger AI anchors

Stories and Projects are important trust pages. Future backend or schema planning should help AI understand:

- Stories = founder/history/philosophy/proof archive
- Projects = project archive / creative work collection

## Safe next actions

Backend-only:

1. Create `SCHEMA_VALIDATION_REPORT.md`.
2. Validate JSON-LD syntax page by page.
3. Confirm each canonical URL matches `sitemap.xml` and `llms.txt`.
4. Confirm `trade.html` remains compatibility-only.
5. Plan possible future schema additions without editing HTML.

Review-first only:

- project fact boxes
- Belong proof blocks
- founder/About proof blocks
- visible captions
- FAQ blocks
- public proof sections

## Do not do during SEO/AI work

- Do not rewrite visible headings.
- Do not rewrite visible paragraphs.
- Do not change buttons.
- Do not change cards or captions.
- Do not change nav labels.
- Do not reorder public page sections.
- Do not add product prices, sizes, exact stock counts, shipping, condition, or purchase terms unless Vaughan verifies them.
- Do not claim architecture, engineering, landscape architecture, or full design-build services.

## Practical next move

The next real value move is `SCHEMA_VALIDATION_REPORT.md`.

That should be a report only. It should not edit HTML. It should identify where schema is strong, where it is weak, and what could be added later under review.
