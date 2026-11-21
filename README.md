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

## Editing content
All text, services, portfolio projects, testimonials, blog posts and contact details are in clearly labelled blocks at the top of the script in `index.html` (`CONFIG`, `IMAGES`, `SERVICES`, `PROJECTS`, `POSTS`, `T`). To use a real photo, add it to `images/` and set that item's `src`.
