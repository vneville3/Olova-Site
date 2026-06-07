# OLOVA Header Logo Test

Date: 2026-06-06

## Asset Copied

Source:

`E:\AAA\REFERENCE\Olova\Logos and Graphic Design\03_Exports_Web\olova-header-icon-white-transparent-temp-2026-06-06.png`

Site asset:

`F:\Apps\OLOVA\Olova-Site\assets\olova-header-icon-white-temp.png`

The copied file is 35,779 bytes. Its SHA-256 matches the source:

`15A0A41FC31A171681B1A6985475501C1ED6282680CB547384941B8A898A330B`

The asset is a temporary 512 x 512 transparent raster, not a final master.

## HTML Files Changed

Visible header image references were updated in:

- `404.html`
- `belong-centre.html`
- `community.html`
- `contact.html`
- `design.html`
- `index.html`
- `products.html`
- `projects.html`
- `stories.html`

The 404 page keeps its root-relative asset path:

`/assets/olova-header-icon-white-temp.png`

All other pages use:

`assets/olova-header-icon-white-temp.png`

No page content, navigation labels, or routes were changed.

## CSS Changed

File:

`assets/styles.css`

The `.brand-mark` wrapper remains 42 x 42px. Padding changed from 8px to 4px so the icon has enough visible area without increasing header height.

No navigation layout or header-height rule changed.

## Structured Data

Home organization structured data remains unchanged:

`https://olovatrading.ca/assets/olova-mark.svg`

The temporary PNG is not referenced by JSON-LD.

## Preview Results

Previewed:

- Home at 1440px desktop
- Home at 390px mobile portrait
- Home at 844px mobile landscape
- 404 page at 390px through a local HTTP server

Screenshots:

- `G:\MiniV\Vaughan-Brain\.codex-work\olova-header-logo-test\home-desktop-1440.png`
- `G:\MiniV\Vaughan-Brain\.codex-work\olova-header-logo-test\home-mobile-390.png`
- `G:\MiniV\Vaughan-Brain\.codex-work\olova-header-logo-test\home-landscape-844.png`
- `G:\MiniV\Vaughan-Brain\.codex-work\olova-header-logo-test\404-mobile-http-390.png`

Visual findings:

- the new icon is clear and recognizable at the live 42px wrapper size;
- it matches the selected refined cube/plaza system more closely than the prior site SVG;
- header height is unchanged;
- mobile portrait navigation remains unchanged;
- mobile landscape navigation still fits;
- the 404 root-relative image path resolves correctly over HTTP;
- the raster is slightly softer than a future SVG master would be, but it is suitable for this temporary test.

## Static Checks

- Exactly nine visible header references use the temporary PNG.
- Home JSON-LD still uses `assets/olova-mark.svg`.
- All local references resolve on the nine changed pages.
- The original `assets/olova-mark.svg` remains in place.
- Favicon, Apple touch icon, and social preview references were not changed.
- No deployment was performed.

## Sizing Follow-Up

Three shared `.brand-mark` options were tested:

- Option A: 48 x 48px wrapper with 3px padding
- Option B: 52 x 52px wrapper with 3px padding
- Option C: 56 x 56px wrapper with 2px padding

Selected:

**Option B: 52 x 52px with 3px padding**

Only `assets/styles.css` and this report were changed during the sizing follow-up. No HTML or logo asset was changed.

The selected CSS is:

```css
.brand-mark{width:52px;height:52px;border-radius:12px;padding:3px;border:1px solid rgba(255,255,255,.08);background:rgba(255,255,255,.02)}
```

The existing compact landscape override remains:

```css
@media (max-width:920px) and (max-height:500px){
  .brand-mark{width:36px;height:36px}
}
```

Visual result:

- 48px was cleaner than the original 42px mark but still restrained.
- 52px gives the icon clear brand presence without overpowering the adjacent OLOVA text.
- 56px begins to compete with the text lockup and sits close to the 72px desktop header limit.
- Desktop header height remains controlled.
- 390px mobile portrait keeps the two-row navigation clear and collision-free.
- 844px mobile landscape remains on the compact 36px override, preserving its single-row header and nav.
- The 404 mobile header also remains balanced.

Final screenshots:

- `G:\MiniV\Vaughan-Brain\.codex-work\olova-header-sizing\selected-b\home-desktop-1440.png`
- `G:\MiniV\Vaughan-Brain\.codex-work\olova-header-sizing\selected-b\home-mobile-390.png`
- `G:\MiniV\Vaughan-Brain\.codex-work\olova-header-sizing\selected-b\home-landscape-844.png`
- `G:\MiniV\Vaughan-Brain\.codex-work\olova-header-sizing\selected-b\404-mobile-390.png`

Remaining concern:

- The temporary raster remains slightly softer than a future SVG master, especially under close inspection. At the selected live size it remains clear and usable.
