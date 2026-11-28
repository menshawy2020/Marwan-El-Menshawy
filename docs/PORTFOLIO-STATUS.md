# Portfolio — media status & pending assets

Merged into `main` and live, approved by Marwan on 2026-11-23.

Preview mode: add `?preview=1` to the address (e.g. `index.html?preview=1#work/charles-american-food`), or `#preview` on hosts that drop query strings (such as the private Claude preview page).
Preview mode shows projects in review, pending-file placeholders and "temporary" labels. The public site hides all three.

## Projects

| Project | Category | Status | Photos live | Cover |
|---|---|---|---|---|
| Emerald Elegance | Fashion & Editorial | Published | 6 | DSC_0078 |
| Champagne Glow | Fashion & Editorial | Published | 7 | DSC_0056 |
| Bridal Editorial (Makeup Artist: Nayera) | Beauty & Makeup | Published, **temporary media** | 10 | WhatsApp 2026-11-20 2.04.05 AM (2) |
| Alexandria Stadium | Architecture & Heritage | Published | 3 (+5 pending) | DSC_0151 |
| Landscape | Landscape | Published | 10 (+1 photo, +1 video pending) | 20260716_194813 |
| Charles American Food | Food & Restaurants | Published | 6 retouched; AI pasta not approved | DSC_0031 retouch |

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

- Landscape: 20250614_192432(2).jpg, 20261021_145449_1.mp4 (video)

Each is listed in `PROJECTS` with `pending: true`. It appears as a labelled placeholder in preview mode only.

## Other notes

- DSC_0030 and DSC_0031 in the Charles folder were byte-identical duplicates (same checksum), so each is used once. Drive originals are untouched.
- Service photos: Event (bridal-08, temporary), Media Coverage (Stadium DSC_0151), Corporate (Stadium DSC_0131), Brand (Charles DSC_0031 retouch), Content Creation (bridal-06, temporary), Behind-the-Scenes (bridal-07, temporary).
- Contact: WhatsApp +20 111 848 4442, marwan.menshawy2026@gmail.com, instagram.com/maro_mensho. LinkedIn removed.
- About portrait: pending an authentic photo of Marwan. The 15-year figure is pending final confirmation.
- Insights: three drafts, hidden from the public site and menu until one is published.
- GPS location data was found in all 10 landscape originals and removed from every web copy.
- The Charles images (two Version A retouches and the AI pasta image) are prepared, but they're not committed. This repository is public, so they stay out until each is approved. In the data they're marked `held: true`.

## Update 2026-11-23 (final)
- Portraits from Drive folder 07-Portrait: hero = 20260911_174611 (suit), About = 20260606_175431 (outdoors), About small = 20260305_085505 (mirror). GPS removed.
- Charles American Food is published with the two approved Version A retouches. The AI pasta image is not approved: it's not on the site and not in the repo.
- 15 years of photography is confirmed by Marwan.

## Update 2026-11-28 — Featured film: The Art of Beauty
- Vertical bridal beauty film (9:16, 25 s, soft sound design, no music, no dialogue), shown as the featured piece at the top of Portfolio, with a full-screen viewer.
- Text and credits are in `FILM` in `index.html` (approved wording; keep spelling): Makeup Artist Naiara El Khatib · Bridal Veil Styling Malak Vel Designer · Photography & Videography Marwan El Menshawy. No client name.
- Media files (add these to the repo; the site points at them):
  - `video/bride-b-modern-beauty-reel.mp4` (1080x1920, larger screens)
  - `video/bride-b-modern-beauty-reel-720.mp4` (720x1280, screens 768 px and below)
  - `images/work/the-art-of-beauty/bride-b-modern-beauty-reel-poster.jpg` (poster)
  - `images/work/the-art-of-beauty/bride-b-modern-beauty-reel-poster-alt.jpg` (used as the Photo & Video Editing service image)
- New service: Photo & Video Editing (7 services in total). VideoObject structured data added in `<head>`.
- Open question: the Bridal Editorial credit says "Nayera"; the film credit says "Naiara El Khatib". Check whether this is the same artist and align the spelling.
