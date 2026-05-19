# OLOVA Site Current Rules

This file records the current operating guardrails after the May 2026 SEO/AI-readability work and homepage recovery. Treat this as the current override when older notes conflict.

## Current implementation

- Public product label: `Products`.
- Canonical product page: `products.html`.
- Compatibility page: `trade.html` redirects to `products.html` and should not be listed in the sitemap.
- `Products` is the settled public nav label for now, even if older notes discuss `Trade` as a possible future label.
- `llms.txt`, `sitemap.xml`, `robots.txt`, SEO audits, visible-copy audit, metadata, JSON-LD, and canonical tags are the current AI/search-readable layer.

## Visible copy freeze

Visible human-facing copy is frozen unless Vaughan explicitly opens a writing or visible-add-on task.

Do not change the following during SEO/AI-readable work:

- visible headings
- visible paragraphs
- button labels
- card text
- captions
- nav labels
- page-flow text
- layout text
- images or video

The current visible writing was produced through a separate writing process and must not be improved, polished, reorganized, or rewritten during technical SEO/AI work.

## Allowed SEO / AI-readable work

The following work is allowed without touching visible page copy:

- update or validate `llms.txt`
- update or validate `sitemap.xml`
- update or validate `robots.txt`
- create or update markdown audits and plans
- validate metadata and JSON-LD
- adjust non-visible canonical links or schema only when required
- produce reports comparing visible copy, metadata, sitemap, schema, or crawlability

## Review-first zone

These are allowed only after Vaughan explicitly approves the specific visible add-on:

- project fact boxes
- role/status proof blocks
- visible proof sections
- FAQ blocks
- public captions
- About / founder content
- Belong proof blocks

These may improve AI readability, but they are visible to humans and therefore belong to a separate approval process.

## Recovery lesson

A recent SEO/AI-readability session accidentally touched `index.html` visible content and caused homepage recovery work. The rule going forward is strict:

SEO/AI-readable work must not freeload visible copy edits.

If an agent or assistant needs to touch an HTML file, it must first state whether the change is visible or invisible. If visible, stop and get Vaughan's explicit approval before editing.

## Safe workflow

- Text-only backend/search files may be edited through GitHub connector or local repo workflows.
- Binary assets still require the safer media workflow and verification.
- For visible copy, use a separate writing session, not the SEO/AI workflow.
- Before committing technical changes, verify changed files do not include unintended public copy edits.
