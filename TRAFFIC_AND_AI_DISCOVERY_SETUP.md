# OLOVA Traffic and AI Discovery Setup

Backend-only planning document. No HTML was edited. No visible copy was changed. No tracking code was installed.

## Purpose

Set up the free/low-friction discovery stack for OLOVA:

1. Google Search Console
2. Google Analytics 4
3. Bing Webmaster Tools
4. Microsoft Clarity, only if appropriate after privacy/youth-audience review

This file is a setup plan, not an implementation.

## Current site readiness

OLOVA is ready for webmaster/search setup because the repo already has:

- `robots.txt`
- `sitemap.xml`
- `llms.txt`
- canonical Products strategy
- current public pages listed in the sitemap
- visible-copy guardrails

## Priority 1: Google Search Console

Goal: tell Google what the site is, submit the sitemap, inspect key URLs, and see search queries/impressions over time.

### Human steps

1. Go to Google Search Console.
2. Add property for `https://olovatrading.ca/`.
3. Prefer Domain verification if DNS access is available.
4. If DNS is annoying, use URL-prefix verification and provide the HTML meta verification tag to the assistant.
5. Submit sitemap:
   - `https://olovatrading.ca/sitemap.xml`
6. Use URL Inspection for:
   - `https://olovatrading.ca/`
   - `https://olovatrading.ca/design.html`
   - `https://olovatrading.ca/community.html`
   - `https://olovatrading.ca/stories.html`
   - `https://olovatrading.ca/products.html`
   - `https://olovatrading.ca/projects.html`
   - `https://olovatrading.ca/belong-centre.html`
   - `https://olovatrading.ca/contact.html`

### What Vaughan should provide if HTML verification is used

Paste the exact Search Console verification meta tag, usually similar to:

```html
<meta name="google-site-verification" content="..." />
```

### Assistant implementation rule

Adding this meta tag is invisible metadata, but it touches HTML. Before installing, confirm the exact tag and edit only `<head>`. Do not alter visible copy.

## Priority 2: Google Analytics 4

Goal: see visitor volume, pages viewed, acquisition source, and basic engagement.

### Human steps

1. Create or open a Google Analytics account.
2. Create a GA4 property for OLOVA.
3. Add a Web data stream for `https://olovatrading.ca/`.
4. Copy either:
   - the Measurement ID, starting with `G-`, or
   - the full Google tag snippet.

### What Vaughan should provide

Either:

```text
G-XXXXXXXXXX
```

or the full Google tag snippet beginning with:

```html
<!-- Google tag (gtag.js) -->
```

### Assistant implementation rule

Install the tag immediately after `<head>` on root HTML pages only after Vaughan provides the ID/snippet and confirms tracking installation.

Do not alter visible copy.

## Priority 3: Bing Webmaster Tools

Goal: give Bing/Microsoft search a clean sitemap and ownership signal. This may also support better visibility in Microsoft search surfaces.

### Human steps

1. Open Bing Webmaster Tools.
2. Add `https://olovatrading.ca/`.
3. If offered, import from Google Search Console after Search Console is verified.
4. Submit sitemap:
   - `https://olovatrading.ca/sitemap.xml`
5. Check crawl/indexing status for the main pages.

### What Vaughan should provide if verification needs HTML

Paste the exact Bing verification meta tag if DNS/import verification is not used.

### Assistant implementation rule

Verification meta tags are invisible metadata but touch HTML. Confirm first. Edit only `<head>`. Do not alter visible copy.

## Priority 4: Microsoft Clarity, optional

Goal: visual user-behavior feedback such as heatmaps, scroll depth, and session recordings.

Important caution: OLOVA includes youth/community content. Clarity should only be used if it is appropriate for the site's audience and privacy posture. If the site is considered targeted at users under 18, do not install Clarity.

### Human decision needed first

Decide whether OLOVA is a site targeting minors globally.

- If yes: skip Clarity.
- If no: Clarity can be considered, with default masking left on and no sensitive form fields added.

### Human steps if approved

1. Create a Microsoft Clarity project for `https://olovatrading.ca/`.
2. Copy the tracking code.
3. Provide the exact script to the assistant.

### Assistant implementation rule

Install Clarity only after Vaughan explicitly approves the privacy/youth-audience decision. Edit only `<head>`. Do not alter visible copy.

## Recommended implementation order

1. Set up Google Search Console.
2. Submit sitemap.
3. Request indexing / inspect the main URLs.
4. Set up GA4.
5. Install GA4 tag after Vaughan provides Measurement ID or snippet.
6. Set up Bing Webmaster Tools.
7. Decide whether Clarity is appropriate.
8. If approved, install Clarity.

## Files likely touched later

Only if verification or tracking snippets are installed:

- `index.html`
- `design.html`
- `community.html`
- `stories.html`
- `products.html`
- `projects.html`
- `belong-centre.html`
- `contact.html`
- possibly `404.html`

These edits must be invisible `<head>` changes only.

## Do not touch

- visible headings
- visible paragraphs
- buttons
- cards
- captions
- images
- videos
- layout
- product claims
- prices, sizes, exact stock counts, shipping, condition, or purchase terms

## Immediate ask for Vaughan

Provide whichever of these you get first:

1. Google Search Console verification meta tag, if needed.
2. GA4 Measurement ID or full Google tag snippet.
3. Bing verification meta tag, if needed.
4. Clarity script only after deciding the youth/privacy issue.
