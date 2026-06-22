# Anchorline Business Solutions — website project

A 5-page static business/consulting website built with plain HTML, CSS, and vanilla JS (no build step, no framework).

## Structure

```
anchorline/
├── index.html        Home
├── services.html      Services (advisory, digital & web, operations)
├── about.html          About / story / values / timeline
├── why-us.html          Stats, comparison table, testimonials
├── contact.html          Contact form + info
├── css/style.css        All styles (design tokens at the top)
└── js/main.js            Nav toggle, FAQ accordion, scroll reveal, route-line draw, demo form
```

## Running it

No build tools needed. Just open `index.html` in a browser, or serve the folder locally:

```bash
cd anchorline
python3 -m http.server 8000
# visit http://localhost:8000
```

## Customizing

- **Colors & type**: edit the CSS custom properties at the top of `css/style.css` (`:root`).
- **Copy**: all text lives directly in the HTML files — no CMS or data layer.
- **Images**: currently hot-linked from Unsplash for placeholder purposes. Swap the `<img src="">` values for your own hosted images before going live.
- **Contact form**: `contact.html` submits to nothing — it shows a success message client-side only (see `js/main.js`). Wire it to a real endpoint (Formspree, your own backend, etc.) before launch.

## Notes

- Fonts (Fraunces, Inter, IBM Plex Mono) load from Google Fonts via `@import` in `style.css`.
- Fully responsive, keyboard-focus visible, and respects `prefers-reduced-motion`.
