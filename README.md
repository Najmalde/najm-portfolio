# Najm Aldeen — Bilingual Professional Portfolio

A lightweight, responsive portfolio built with semantic HTML, CSS, and vanilla JavaScript. It does not require a build step or third-party JavaScript dependencies.

## Features
- English and Arabic language switching with RTL/LTR layout changes.
- Language preference persistence using localStorage (with safe fallbacks).
- Dark/light theme switch with saved preference and system-theme fallback.
- Responsive sticky navigation and active-section indication.
- Accessible project detail dialogs with Escape/close behavior and focus return.
- Filterable skill categories.
- Subtle reveal animations that respect reduced-motion settings.
- Back-to-top control.
- CV download, email, and telephone links.
- Local profile photo, favicon, and CV assets.

## Run locally
1. Extract the ZIP archive.
2. Open `index.html` in a browser, or serve the folder with a local static server.
3. For example, run `python -m http.server 8000` from this directory and open `http://localhost:8000`.

## Deploy
Upload the project folder to a static hosting provider such as Netlify, Vercel, or GitHub Pages. Keep `assets/` beside `index.html`.

## Before publishing
- Confirm the displayed CV details and Arabic wording.
- Add verified GitHub and LinkedIn URLs if desired.
- Add repository/demo links only when real URLs are available.
- The contact CTA uses `mailto:` and opens the visitor's email application; it does not submit to a backend.
- The existing portfolio address is not presented as a verified live demo link.
- Run Lighthouse on the deployed site to measure actual performance. No Lighthouse score is claimed without testing.

## Architecture
- `index.html` — semantic page content and interaction containers.
- `styles.css` — responsive layout, theme tokens, RTL support, and motion styles.
- `script.js` — translations, theme, navigation, skill filters, project dialogs, and scroll interactions.
- `assets/profile.webp` — optimized profile image.
- `assets/najm-aldeen-cv.pdf` — downloadable CV.
- `assets/favicon.svg` — custom favicon.

## Validation performed
- JavaScript syntax check (`node --check`).
- Checked that all internal `#section` links have matching IDs.
- Checked that all referenced local assets exist.

Browser-based interaction tests and Lighthouse audits have not been run in this environment.
