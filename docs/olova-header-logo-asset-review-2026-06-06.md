# OLOVA Header Logo Asset Review

Date: 2026-06-06

## Decision

The current `assets/olova-mark.svg` is usable as a temporary header mark, but it is not the best match for the selected refined OLOVA system.

It is crisp and legible, but:

- it includes its own dark rounded-square background;
- its cube and chevron geometry is an earlier simplified interpretation;
- it does not exactly match the icon-only mark shown in the selected refined lockup system.

Two temporary icon-only raster assets were therefore created for header testing.

## Temporary Assets Created

White icon for the current dark website header:

`E:\AAA\REFERENCE\Olova\Logos and Graphic Design\03_Exports_Web\olova-header-icon-white-transparent-temp-2026-06-06.png`

Black icon for possible future light-background use:

`E:\AAA\REFERENCE\Olova\Logos and Graphic Design\03_Exports_Web\olova-header-icon-black-transparent-temp-2026-06-06.png`

Both files are:

- 512 x 512 PNG;
- icon-only;
- transparent;
- tightly padded;
- free of baked backgrounds and glow;
- temporary raster derivatives, not final masters.

The artwork was isolated from the icon-only panel in:

`E:\AAA\REFERENCE\Olova\Logos and Graphic Design\ChatGPT Image Jun 6, 2026, 08_42_20 PM.png`

No files were added to `01_Final_Logo_System`.

## Preview Sheet

PNG comparison:

`E:\AAA\REFERENCE\Olova\Logos and Graphic Design\03_Exports_Web\olova-header-icon-comparison-preview-2026-06-06.png`

HTML source:

`E:\AAA\REFERENCE\Olova\Logos and Graphic Design\03_Exports_Web\olova-header-icon-comparison-preview-2026-06-06.html`

The sheet compares:

- current site SVG;
- proposed white transparent icon;
- proposed black transparent icon;
- 42px, 64px, and 128px sizes;
- dark and light backgrounds.

## Recommendation

Use the new white temporary icon in a later, narrowly scoped header test.

Do not overwrite `assets/olova-mark.svg`. Copy the temporary white PNG into the site under a distinct filename so the current SVG remains an immediate fallback.

The existing header wrapper is `42px` square with `8px` padding. That leaves only about `26px` for the image. When testing the new icon, reduce wrapper padding to approximately `4px` or `5px` so the icon reads clearly without increasing header height.

Keep the current adjacent text lockup:

- `OLOVA`
- `Skater-Owned . Tri-Cities, BC`

Do not add the full arched wordmark to this compact header.

## Quality Concerns

- The proposed icons were extracted from a raster concept sheet and enlarged to 512px.
- They are clean enough at the reviewed web sizes, especially 42px and 64px, but show raster softness at larger inspection sizes.
- They must not be treated as final vector or print masters.
- A proper SVG icon master should eventually replace them.
- The black variant is intended for light backgrounds and disappears on the current dark header.
- The white variant is intended for the current dark header and disappears on light backgrounds.

## Website Editing

A header-only implementation can proceed after approval, using the white temporary icon and a small `.brand-mark` padding adjustment.

That later pass should:

- copy only the white temporary icon into `assets`;
- update header image references;
- preserve header dimensions and navigation;
- leave favicon, Apple touch icon, social previews, and structured data unchanged;
- preview desktop, mobile portrait, and mobile landscape;
- retain `assets/olova-mark.svg` as a fallback.

No website HTML, CSS, structured data, favicon, social preview, or existing site logo asset was changed during this review.
