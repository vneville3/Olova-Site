# Website publishing workflow notes

## What failed
The GitHub app route successfully accepted commits, but binary media blobs became corrupted after upload. That affected JPG and MP4 assets and caused broken images and video on the live site.

## What worked
- HTML and CSS committed as plain UTF-8 text
- Local image selection through chat uploads
- Local optimization and naming before publish
- GitHub Pages serving existing repo assets correctly when those assets are valid

## Safe workflow going forward
1. Keep Google Drive as archive and source library.
2. Use chat uploads for real image and video selection.
3. Optimize and rename publish-ready files locally.
4. Commit HTML and CSS through plain UTF-8 text only.
5. Upload images and video directly to the GitHub repo `assets/` folder through GitHub web when the GitHub app binary route is not verified.
6. Reuse stable filenames so page HTML does not need repeated edits.
7. After any binary upload, verify one asset in the repo before assuming the whole batch is good.

## Current media filenames in use
- assets/products-spine-hero-v01.jpg
- assets/products-spine-side-detail-v01.jpg
- assets/products-spine-close-detail-v01.jpg
- assets/products-spine-packaging-detail-v01.jpg
- assets/products-spine-lifestyle-v01.jpg
- assets/contact-vaughan-skater-owned-v01.jpg
- assets/design-zambia-flythrough-poster-v01.jpg
- assets/design-zambia-flythrough-v01-small.mp4

## Immediate rule
Text through app. Binary through direct repo upload unless proven safe.
