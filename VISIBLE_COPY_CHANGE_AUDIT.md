# Visible Copy Change Audit

## Scope

Read-only audit of visible, human-facing copy changes from the SEO/AI-readability work window.

Comparison baseline:

- Baseline ref: `3f4da4fd1e861609c5867dc95c6213bcb3ab2574`
- Reason: last commit found immediately before the SEO/AI-readability commit sequence began on May 17, 2026.
- Current ref: `main` at time of audit.

Pages checked:

- `index.html`
- `products.html`
- `design.html`
- `community.html`
- `stories.html`
- `projects.html`
- `belong-centre.html`
- `contact.html`

This audit separates visible page copy from metadata, canonical tags, sitemap, `llms.txt`, robots, and JSON-LD/schema changes.

## Summary

Visible copy changed materially on:

- `index.html`
- `products.html`

Visible copy changed only in navigation label/route on:

- `design.html`
- `community.html`
- `stories.html`
- `projects.html`
- `contact.html`

No visible copy changes found on:

- `belong-centre.html`

## Backend / Metadata / Schema Changes Not Counted As Visible Copy

The full repo comparison from the pre-SEO baseline to current `main` includes backend or AI/SEO-facing work outside this visible-copy audit:

- `SEO_AI_READABILITY_AUDIT.md` added.
- `TRUTH_LAYER_AUDIT.md` added.
- `llms.txt` added.
- `sitemap.xml` updated.
- `trade.html` changed into a compatibility redirect path.
- JSON-LD/schema and metadata were added or changed on multiple pages.
- Product canonical strategy changed so `products.html` is canonical and `trade.html` redirects to Products.

Those changes are not treated as human-facing visible copy except where they changed visible navigation labels, buttons, page text, headings, captions, cards, or fallback page text.

## Page-by-Page Visible Copy Changes

## `index.html`

`index.html` has major visible copy changes. The current visible homepage copy reflects the restored April 8 human-facing version while keeping the current Products route.

Changed navigation:

- Removed visible nav label/link: `Trade` -> `trade.html`
- Added visible nav label/link: `Products` -> `products.html`

Changed hero copy:

- Eyebrow changed from `Skater-led by Vaughan Smith-Neville` to `Skater-owned and operated`.
- H1 changed from `Skatepark design, public-space thinking, and real local backing.` to `Selective products, skatepark design, and local projects rooted in the Tri-Cities.`
- Lead paragraph changed from Vaughan/public-home-base design/community wording to:
  `OLOVA handles selective products, skatepark and public-space concepts, and local projects worth backing. Rooted in Port Moody, Coquitlam, and Port Coquitlam, the company stays lean, direct, and hands-on.`
- Secondary hero button changed from `See community work` to `See SPINE` and now links to `products.html`.

Changed first section / lane cards:

- Section headline changed from `Design leads. Community proves it.` to `A tight scope, kept intentional.`
- Section note changed from `Concept work, local involvement, and a smaller trade lane that stays secondary.` to `Products, design work, and local project support that fit the same point of view.`
- Card 01 changed from `Design` to `Products`.
- Card 01 paragraph changed to `Selective product handled directly from BC. Right now that means the remaining Canadian SPINE stock.`
- Card 01 link changed from `Open design` to `See products`.
- Card 02 changed from `Community` to `Design and Visualization`.
- Card 02 paragraph changed to concept design / visual development wording.
- Card 02 link changed to `Open the design page`.
- Card 03 changed from `Trade` to `Community`.
- Card 03 paragraph changed to local project / youth space / skate advocacy wording.
- Former `See trade` link was removed.

Changed current focus section:

- Kicker changed from `Best fit` to `Current focus`.
- Heading changed from `Early-stage projects that need a sharper read.` to `Design work, local support, and remaining SPINE stock.`
- Paragraph changed from early-stage project clarity wording to current public-space design, local support, and SPINE inventory wording.
- Pills changed from design-service terms to:
  - `Tri-Cities based`
  - `SPINE available`
  - `Skatepark and plaza design`
  - `Belong support`
  - `Local project work`
- Link changed from `See selected work` to `See current product focus`.

Changed rooted locally section:

- Section kicker changed from `Proof on the ground` to `Rooted locally`.
- Section headline changed from `Local roots matter.` to `The local footing is part of the point.`
- Section note changed to name Port Moody, Coquitlam, and Port Coquitlam directly.
- First media card changed from `Community work with real stakes` to `Local project support`.
- First card paragraph changed to Belong / wider Tri-Cities indoor space, youth access, and local skate infrastructure wording.
- Second media card changed from a Stories / point-of-view card to a design-range card:
  - Heading changed from `A skatepark does not always need to look like one.` to `Range without the noise`.
  - The two previous paragraphs about history, advocacy roots, and public places were replaced by one paragraph about design range across civic concepts, landscape thinking, and skate-focused environments.

Changed contact panel:

- Heading changed from `Got a project that needs a sharper read?` to `Start with the right conversation.`
- Paragraph changed from project-site/context inquiry wording to product/design/community conversation wording.
- Mailto subject changed from `OLOVA Project Inquiry` to `OLOVA Inquiry`; visible email label remains the same.
- Footer second line changed from `Design, community, and selective product` to `Skater-owned and operated`.

Potential Vaughan review:

- The restored homepage is more product-forward than the pre-SEO baseline. It explicitly leads with `Selective products` and names SPINE in the hero button and current-focus section.
- The previous homepage positioned design/community first; the current homepage presents Products first in the lane cards.
- The newer story/advocacy framing on the homepage was removed from the visible second media card.

## `products.html`

`products.html` changed from a redirect/fallback page into a full visible Products page.

Removed visible copy:

- `Redirecting to Trade …`

Added visible navigation:

- `Home`
- `Design`
- `Community`
- `Stories`
- `Products`
- `Contact`

Added hero copy:

- Eyebrow: `Products`
- Eyebrow: `Small, honest, secondary`
- H1: `Select product handled without pretending it is the whole company.`
- Lead paragraph explaining Products as the support lane under OLOVA and naming remaining Canadian odd CIRKUS SPINE Black/Grey stock already in BC.
- Buttons: `Ask about current stock`, `See the main design work`.

Added current reality section:

- Kicker: `Current reality`
- Heading: `What is actually here`
- Paragraph about no giant catalog, no fake wholesale theater, remaining Canadian SPINE stock, and direct inquiry from British Columbia.
- List items:
  - `Brand: odd CIRKUS`
  - `Model: SPINE Black/Grey`
  - `Availability: remaining pairs only`
  - `Handled from: British Columbia`
  - `Purchase path: direct inquiry`

Added page-purpose section:

- Kicker: `Why this page exists`
- Heading: `Product stays visible, but in its place.`
- Paragraph about not burying real product and not letting product hijack the identity.

Added SPINE section:

- Kicker: `Current item`
- Heading: `SPINE is the live chapter, not the whole book.`
- Section note: `The pair is real. The lane is real. The scale is still intentionally modest.`
- Product card headings: `Shape from the side`, `Better judged on foot`.
- Product card paragraphs about silhouette, lace setup, loud branding, on-foot proof, and avoiding forced sales language.

Added contact panel:

- Heading: `Need a size check or product conversation?`
- Paragraph: `Send your size, city, and what you are after. The answer should stay direct.`
- Visible email button: `vneville@olovatrading.ca`.

Potential Vaughan review:

- This is the largest visible change after the homepage.
- It adds public product facts around remaining SPINE stock, availability as `remaining pairs only`, BC handling, and direct inquiry.
- It adds a clear brand/product narrative that did not exist visibly on `products.html` at the baseline because that page was only redirecting to Trade.
- Any commerce-adjacent details should remain reviewed by Vaughan before adding prices, sizes, stock counts, condition, shipping, or purchase terms.

## `design.html`

Visible body copy did not change except the main navigation label and route.

Changed visible navigation:

- Removed: `Trade` -> `trade.html`
- Added: `Products` -> `products.html`

No changed visible headings, body paragraphs, buttons, project captions, cards, or section copy were found.

Potential Vaughan review:

- Confirm that `Products` is still the desired public nav label instead of `Trade`.

## `community.html`

Visible body copy did not change except the main navigation label and route.

Changed visible navigation:

- Removed: `Trade` -> `trade.html`
- Added: `Products` -> `products.html`

No changed visible headings, body paragraphs, buttons, captions, cards, or section copy were found.

Potential Vaughan review:

- Confirm that `Products` remains the correct public nav label on community-facing pages.

## `stories.html`

Visible body copy did not change except the main navigation label and route.

Changed visible navigation:

- Removed: `Trade` -> `trade.html`
- Added: `Products` -> `products.html`

No changed visible headings, body paragraphs, buttons, captions, cards, or section copy were found.

Potential Vaughan review:

- Confirm that product wording in navigation does not pull the Stories page away from its trust/history role.

## `projects.html`

Visible body copy did not change except the main navigation label and route.

Changed visible navigation:

- Removed: `Trade` -> `trade.html`
- Added: `Products` -> `products.html`

No changed visible project headings, body paragraphs, buttons, captions, cards, or archive copy were found.

Potential Vaughan review:

- Confirm `Products` as the nav label across project/archive contexts.

## `belong-centre.html`

No visible copy changes found.

The visible nav, headings, paragraphs, buttons, cards, captions, and footer copy matched the baseline for this page.

Potential Vaughan review:

- None from this visible-copy comparison.

## `contact.html`

Visible body copy did not change except the main navigation label and route.

Changed visible navigation:

- Removed: `Trade` -> `trade.html`
- Added: `Products` -> `products.html`

No changed visible headings, body paragraphs, buttons, cards, or section copy were found.

Potential Vaughan review:

- Confirm `Products` as the nav label on the primary conversion page.

## What Did Not Change Visibly

- `belong-centre.html` visible copy did not change.
- `design.html`, `community.html`, `stories.html`, `projects.html`, and `contact.html` did not show visible body-copy changes beyond the `Trade` to `Products` navigation label/route.
- No visible project archive copy changed on `projects.html` except navigation.
- No visible Belong story/body copy changed on `community.html` except navigation.
- No visible contact body copy changed on `contact.html` except navigation.

## Changes That May Need Vaughan Review

- Homepage strategy: current `index.html` is more Products-forward than the pre-SEO baseline and puts Products first in the cards.
- Homepage proof layer: the previous homepage story/history card was removed from visible copy during the restore; decide whether that human-memory layer should reappear somewhere.
- Products page: verify all public product statements, especially remaining stock, direct inquiry path, and BC handling.
- Site-wide nav: confirm `Products` is the settled public label over `Trade` across all root pages.
- Product facts still missing by design: price, sizes, exact stock count, shipping, condition, and purchase terms should not be added until Vaughan approves them.
