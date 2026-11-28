# Marwan El-Menshawy — Personal Brand Website & App

Live: https://menshawy2020.github.io/Marwan-El-Menshawy/

A bilingual (English / Arabic) website for photographer and media coverage professional Marwan El-Menshawy. It also works as an installable app (PWA) on iPhone and Android.

## Install as an app
- **iPhone (Safari):** open the site → tap **Share** → **Add to Home Screen**.
- **Android (Chrome):** open the site → tap **Install** on the prompt, or menu **⋮** → **Install app**.

The installed app opens full-screen with its own icon, and pages already visited still load offline.

## Files
| File | Purpose |
|---|---|
| `index.html` | The whole site: content, design and logic |
| `manifest.webmanifest` | App name, icon and colours |
| `sw.js` | Offline support. Bump `VERSION` after editing files so installed apps update |
| `icons/` | App icons |
| `images/` | Photos |
| `video/` | Films (MP4, H.264, faststart). Streamed from the network, never cached by `sw.js` |

## Editing content
All text, services, testimonials, blog posts and contact details are in clearly labelled blocks at the top of the script in `index.html` (`CONFIG`, `IMAGES`, `SERVICES`, `PROJECTS`, `POSTS`, `T`).

## Portfolio projects
- Each project in `PROJECTS` has its own page at `#work/<id>`, with its own gallery and full-screen viewer.
- Photos are served as responsive WebP from `images/work/<project>/<name>-<width>.webp` (about 800/1600/2400 px, never upscaled, metadata removed).
- `status: "review"` keeps a project off the public site. Add `?preview=1` to the address to review it.
- Per image: `treatment` (`original`, `retouched`, `ai-elements`), `temporary: true` for provisional files, `pending: true` for files not received yet.
- Empty `date`, `client` and `desc` fields are hidden automatically.
- Current media status and pending files: see `docs/PORTFOLIO-STATUS.md`.

## Featured film
- `FILM` in `index.html` holds the title, subtitle, description and credits of the featured film at the top of Portfolio.
- The video loads only when it scrolls into view (720p file on screens 768 px and below, 1080p above), plays muted, and pauses off-screen. With reduced motion it shows the poster and a play button.

## SEO
- Keyword research (English and Arabic): `docs/seo/KEYWORD-RESEARCH.md`, with a spreadsheet copy in `docs/seo/keyword-research.csv`.
- `sitemap.xml` lists the site's pages. Add each new page there; it is submitted in Google Search Console.
