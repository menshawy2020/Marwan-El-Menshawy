# Portfolio — media status & pending assets

Branch: `portfolio-real-projects` · Not merged into `main`, so the live site is unchanged.

Preview on a local copy or after merge with `?preview=1` (e.g. `index.html?preview=1#work/charles-american-food`).
Preview mode shows projects in review, pending-file placeholders and "temporary" labels. The public site hides all three.

## Projects

| Project | Category | Status | Photos live | Cover |
|---|---|---|---|---|
| Emerald Elegance | Fashion & Editorial | Published | 6 | DSC_0078 |
| Champagne Glow | Fashion & Editorial | Published | 7 | DSC_0056 |
| Bridal Editorial (Makeup Artist: Nayera) | Beauty & Makeup | Published, **temporary media** | 10 | WhatsApp 2026-11-20 2.04.05 AM (2) |
| Alexandria Stadium | Architecture & Heritage | Published | 3 (+5 pending) | DSC_0151 |
| Landscape | Landscape | Published | 10 (+1 photo, +1 video pending) | 20260716_194813 |
| Charles American Food | Food & Restaurants | **Review — hidden from public** | 0 (2 retouched + 1 AI held for approval, 4 pending) | DSC_0031 retouch (held) |

## Image treatment

| Label | Meaning | Images |
|---|---|---|
| Original | Optimised only (resize, WebP, metadata removed). No edits | Emerald, Champagne, Stadium, Landscape |
| Temporary | WhatsApp-compressed copies, replace with camera originals | Bridal (all 10) |
| Retouched | Conventional colour & light grade on the original photo (Version A) | Charles DSC_0030, DSC_0031 |
| AI-composited | None. Version B was tested and rejected (see below) | none |
| Contains AI-generated elements | Labelled on the site, never a cover, last in gallery, hidden until approved | "Golden Baked Pasta with Bubbly Cheese.png" |

Version B (background composite) was rejected. Automatic subject masking left out the chef's gloved hand (DSC_0030) and cut through the pan rim (DSC_0031), so both would have been altered. That breaks the rule to preserve hands and utensils.

## Pending assets (over Google Drive connector's 10 MB limit)

- Alexandria Stadium: DSC_0060, DSC_0089, DSC_0083, DSC_0128, DSC_0147
- Charles American Food: DSC_0003, DSC_0032, DSC_0068, DSC_0070
- Landscape: 20250614_192432(2).jpg, 20261021_145449_1.mp4 (video)

Each is listed in `PROJECTS` with `pending: true`. It appears as a labelled placeholder in preview mode only.

## Other notes

- DSC_0030 and DSC_0031 in the Charles folder were byte-identical duplicates (same checksum), so each is used once. Drive originals are untouched.
- GPS location data was found in all 10 landscape originals and removed from every web copy.
- The Charles images (two Version A retouches and the AI pasta image) are prepared, but they're not committed. This repository is public, so they stay out until each is approved. In the data they're marked `held: true`.
