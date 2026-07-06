# OLOVA Design Page Local Apply Report

Apply date: 2026-07-05

Target local working site:

`F:\Apps\OLOVA\Olova-Site`

Source patched sandbox:

`F:\Hermes-Sandbox\Builder-Lab\Olova-Site-Test`

Patch package reference:

`F:\Hermes-Sandbox\Builder-Lab\Olova-Site-Test\_olova-patch-package-design-page-restructure-2026-07-05`

## Files Backed Up

Backup folder:

`F:\Apps\OLOVA\Olova-Site\_olova-local-backups\design-page-before-restructure-2026-07-05`

Backed up:

- `design.html`
  - SHA-256: `837CF120A2514E84AD28DC5D235A9BEF7D333DDAC3C8B928736CB0E5168428E9`
- `styles.css`
  - SHA-256: `AE60CE2E2A0C0C08AC4C61EBE284DF636BCDAC966522F8DABB97B78053F9C0A4`

## Files Copied

Copied from sandbox to local working site:

- `design.html`
  - Target SHA-256: `5C3CF75DD809C3C85A173F63F6D657BAD8F0E06F5ADCF45786C57E53F80EF46E`
- `assets\styles.css`
  - Target SHA-256: `5DC19BCEE0D2495A2636B9696C701E6EA8026531A9AB19F37D984CD62F9F97E5`
- `assets\olova-design-video14-slow-cut-720p.mp4`
  - Target SHA-256: `0D82052426100F6C09D8F92D7F378F23A6A7847720B106702809E7C519423B7E`
- `assets\olova-video14-poster.jpg`
  - Target SHA-256: `A1F457418F6D6B567CED8052F365AB5C29FA04591B2BAD5B8356FACE7A519873`

All four copied target files matched the patched sandbox source hashes after copy.

## Validation Results

Temporary validation server:

`http://127.0.0.1:8766/design.html`

The server was stopped after validation.

### File Existence

Confirmed present after copy:

- `F:\Apps\OLOVA\Olova-Site\design.html`
- `F:\Apps\OLOVA\Olova-Site\assets\styles.css`
- `F:\Apps\OLOVA\Olova-Site\assets\olova-design-video14-slow-cut-720p.mp4`
- `F:\Apps\OLOVA\Olova-Site\assets\olova-video14-poster.jpg`

### Browser Validation

Desktop, 1366 x 900:

- No horizontal overflow: pass
- Product nav present: pass
- No Design-page Trade reference: pass
- Video path local: pass, `assets/olova-design-video14-slow-cut-720p.mp4`
- Video muted: pass
- Video poster present: pass, `assets/olova-video14-poster.jpg`
- Video controls visible/enabled: pass
- Video not in hero: pass
- Slava Plaza split into multiple media/copy/card units: pass
- No dual-language blocks: pass
- Broken images: none

Tablet, 768 x 900:

- No horizontal overflow: pass
- Product nav present: pass
- No Design-page Trade reference: pass
- Video path local: pass
- Video muted: pass
- Video poster present: pass
- Video controls visible/enabled: pass
- Video not in hero: pass
- Slava Plaza split into multiple media/copy/card units: pass
- No dual-language blocks: pass
- Broken images: none

Mobile, 390 x 844:

- No horizontal overflow: pass
- Product nav present: pass
- No Design-page Trade reference: pass
- Video path local: pass
- Video muted: pass
- Video poster present: pass
- Video controls visible/enabled: pass
- Video not in hero: pass
- Slava Plaza split into multiple media/copy/card units: pass
- No dual-language blocks: pass
- Broken images: none

## Static Source Checks

Changed runtime files checked:

- `design.html`
- `assets\styles.css`

Results:

- No `E:\AAA` reference in changed runtime files.
- No `Trade` reference in `design.html` or `assets\styles.css`.
- No direct reference to `E:\AAA\REFERENCE\Olova\Website\assets-approved\Design\olova_video14_delivery` in the local site outside backups.
- No `olova_video14_delivery` reference in the local site outside backups.

## Warnings

A broader site scan found pre-existing `E:\AAA` references in docs files unrelated to this Design page patch:

- `docs\olova-header-logo-asset-review-2026-06-06.md`
- `docs\olova-header-logo-test-2026-06-06.md`

These were not introduced by this apply step and were not edited.

## Rollback Instructions

To roll back this local working-site apply:

1. Copy this backup file over the active Design page:
   - From: `_olova-local-backups\design-page-before-restructure-2026-07-05\design.html`
   - To: `design.html`
2. Copy this backup file over the active stylesheet:
   - From: `_olova-local-backups\design-page-before-restructure-2026-07-05\styles.css`
   - To: `assets\styles.css`
3. If fully reverting the Design page video addition and the assets are not needed elsewhere, remove:
   - `assets\olova-design-video14-slow-cut-720p.mp4`
   - `assets\olova-video14-poster.jpg`

## Deployment Confirmation

No deployment was performed.

No commit was created.
