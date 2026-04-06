# OLOVA Website Operating Memory and Guardrails

## Read this first
This file is the long-running operating memory for the OLOVA website. Read it at the start of every new session before making copy, asset, or publishing decisions. Keep it updated as the workflow improves.

## Canonical locations
- Website Drive folder: `Website` in Google Drive
- Drive docs to search by exact title:
  - `Website Notes`
  - `Website Handoff`
- GitHub repo: `vneville3/Olova-Site`
- Repo memory files:
  - `OLOVA_SITE_NOTES.md`
  - `OLOVA_SITE_HANDOFF.md`

## What OLOVA is
- OLOVA is a skater-owned company rooted in the Tri-Cities of British Columbia.
- The website is built around three connected lanes:
  1. selective products
  2. design and visualization
  3. community-linked work
- The company should read as local, selective, hands-on, and real.

## What OLOVA is not
- Not a vague umbrella with abstract lane language leading the public copy.
- Not a full-service municipal design-build skatepark firm.
- Not an interior design company.
- Not a broad catalog distributor.
- Not a fake-startup hype brand using scarcity language to cover weak positioning.
- Not a corporate placemaking consultancy.

## Current business reality
### Products
- odd CIRKUS is no longer an active growth lane.
- Current product reality is the remaining Canadian SPINE stock already in BC.
- Product copy should be honest, direct, and grounded in real availability.
- Better framing: selective product handled directly from BC, limited stock, direct inquiry.
- Avoid writing as though a full future catalog already exists.

### Design
- Strongest design lane is skateparks, plazas, public-space concepts, and visual development.
- Best fit: concept design, 3D visualization, design review, early-stage planning.
- Do not imply licensed architecture or engineering.
- Do not market to interiors or skate shop buildouts as a core lane.

### Community
- Community lane exists because local projects, youth space, advocacy, and Belong matter.
- It is a supporting lane, not the main revenue engine.
- Belong is the clearest current example.
- Tone should be real and measured, not sentimental and not self-congratulatory.

## Writing guardrails
### Core voice
- Skater-owned, local, serious, clear.
- Sound like a real company run by someone who actually knows skating and public-space work.
- Lean toward plainspoken confidence over polished fluff.
- Prefer concrete nouns and real specifics over abstract framework language.

### What to avoid
- `What this lane is now`
- `Where this page earns its keep`
- `This page now reflects...`
- `A few lanes` used as internal architecture talk
- Copy that explains the site to ourselves instead of speaking to the public
- Overclaiming scale or pretending to be a larger firm than OLOVA is
- Fake scarcity, inflated hype, or forced youth slang
- Generic AI polish, consultant phrasing, and mission-statement fog

### What to aim for
- Quartersnacks clarity and groundedness
- Free Skate Mag intelligence and public-space literacy
- Thrasher confidence in measured doses
- The user's own lived voice, organized and distilled
- Public-facing writing that sounds like someone with taste and real involvement wrote it

### Copy process
- The user can write well when organized.
- Assistant’s role is to extract, structure, and sharpen the user’s real language.
- First do a best-effort public pass to remove obvious placeholder language.
- Then narrow page by page through pointed questions.
- Work from top-down:
  1. first screen
  2. first section
  3. supporting sections
  4. CTA and footer polish

## Research guardrails
Always research live when freshness matters.

### Recent market direction already identified
- Established skatepark firms sell broader community outcomes, not just skate features.
- BC recreation language currently emphasizes inclusion, belonging, barrier reduction, youth access, and public-space value.
- Indie skate footwear climate is difficult, and DTC/community-led selling is often more realistic than broad wholesale assumptions.

### Strategic implication
- OLOVA should not try to sound like a giant design-build municipal firm.
- OLOVA’s strongest niche is:
  - skater-owned
  - Tri-Cities rooted
  - concept and design capable
  - community aware
  - selective on products
  - honest about scale

## Technical workflow guardrails
### Reliable workflow
- Google Drive = archive and source library
- Chat uploads = real visual selection and decision-making
- Local optimization and packaging = publish prep
- GitHub app = safe for HTML and CSS text when committed as plain UTF-8
- GitHub web upload = safer path for final JPG and MP4 binaries

### Known failure
- GitHub app binary blob route corrupted JPG and MP4 assets.
- Do not trust binary media publishing through that route unless an individual asset is verified afterward.

### Current safe publish rule
- Text through GitHub app
- Binaries through GitHub web upload to assets unless verified safe

### Media workflow
1. User uploads strong candidate images in chat
2. Assistant selects winners
3. Assistant resizes, compresses, and names publish-ready versions
4. Assistant updates HTML paths and copy
5. User uploads final binary pack to repo assets if needed
6. Verify live render after upload

### HTML workflow
- Commit HTML as plain UTF-8 text only.
- If page corruption appears, re-commit immediately as clean text.
- After copy passes, hard refresh live site to verify.

## Current site status
- Site is now beyond placeholder-framework stage, but still needs continued tightening.
- Home, Products, Community, Design, and Contact all received public-facing copy passes.
- Products had the worst internal-note energy and has been substantially cleaned up.
- Contact image of Vaughan had a broken-media issue at one point; keep an eye on contact page media.
- Overall goal now is refinement, not rescue.

## Current page intent
### Home
- First impression should feel local, skater-owned, selective, and real.
- Avoid over-explaining company architecture.
- Lead with Tri-Cities roots, product/design/community scope, and clear tone.

### Products
- Current product page is about SPINE availability in Canada through OLOVA.
- Keep it grounded in real inventory, direct handling, and clear product views.
- Avoid strategy language and meta-writing.

### Design
- Best public framing: skatepark, plaza, and public-space concepts plus visualization.
- Keep scope honest.
- Municipal and nonprofit readers should find it credible.
- Zambia flythrough is a useful supporting asset, not the center of the page.

### Community
- Belong is the anchor example.
- Tone should show real backing and local connection without turning community into a branding prop.

### Contact
- One inbox, simple routing, strong first impression.
- Should feel direct and presentable even if an image goes missing.

## Asset filenames currently in use
- `assets/products-spine-hero-v01.jpg`
- `assets/products-spine-side-detail-v01.jpg`
- `assets/products-spine-close-detail-v01.jpg`
- `assets/products-spine-packaging-detail-v01.jpg`
- `assets/products-spine-lifestyle-v01.jpg`
- `assets/contact-vaughan-skater-owned-v01.jpg`
- `assets/design-zambia-flythrough-poster-v01.jpg`
- `assets/design-zambia-flythrough-v01-small.mp4`

## Start-of-session checklist
1. Read this file.
2. Check `OLOVA_SITE_HANDOFF.md`.
3. Inspect latest repo state in `vneville3/Olova-Site`.
4. Confirm whether today is copy, media, publishing, or research.
5. For copy work, start with the first thing visitors see.
6. For media work, ask for chat uploads of shortlisted candidates.
7. For publishing, separate text from binary workflow.

## Update protocol
After each meaningful session, update this file with:
- what changed
- what failed
- what new rule was learned
- what still needs work

## Change log
### 2026-04-05
- Rebuilt site copy repeatedly to remove placeholder and notes-to-self language.
- Confirmed GitHub app binary route can corrupt media files.
- Locked working rule: text through GitHub app, binaries through direct upload unless verified.
- Established Drive plus chat uploads plus asset pack workflow.
- Researched current municipal and skate climate to sharpen positioning.
