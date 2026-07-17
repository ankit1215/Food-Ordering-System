# Pizza Restaurant — Responsive Website

A responsive, accessible one-page restaurant site built with semantic HTML5, CSS, and Bootstrap's carousel component.

## Files
- `index.html` — page markup (header, hero, About Us, Menu, Carousel, Gallery, Find Us, footer)
- `style.css` — all styling, including responsive breakpoints
- `script.js` — mobile navigation toggle
- `assets/favicon.svg` — site favicon

## What's implemented
- **Header** — fixed to the top, restaurant logo, `<nav>` with `aria-label`, a mobile menu button with `aria-expanded`/`aria-controls`, and social icons.
- **Hero** — CSS `background` image with a gradient overlay for text contrast.
- **About Us** — two-column semantic `<section>` with an image and copy, stacks on mobile.
- **Menu** — six `<li>` items inside a `role="list"`, each with an image, heading and description.
- **Carousel** — Bootstrap 5 carousel with 5 images, indicators, and prev/next controls with visually-hidden labels.
- **Gallery** — CSS Grid matching the Figma layout (large image + 2×3 grid), reflows to 2 columns on mobile.
- **Find Us** — flex/grid layout with a Google Maps `<iframe>` embed and contact details.
- **Footer** — semantic `<footer>` with logo, nav, contact info and social links.
- **Accessibility** — semantic landmarks (`header`, `main`, `nav`, `footer`, `section`), alt text on every image, ARIA attributes on interactive elements, and visible `:focus-visible` outlines. `prefers-reduced-motion` is respected.
- **Responsive design** — fluid layout down to small mobile widths using CSS Grid/Flexbox and media queries at 900px and 760px.

## Running locally
Just open `index.html` in a browser — no build step required.

## Deploying to GitHub Pages
1. Create a new GitHub repository (e.g. `pizza-restaurant`).
2. Push these files to the repo's `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: pizza restaurant site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/pizza-restaurant.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
5. Save. Your site will be live at:
   `https://<your-username>.github.io/pizza-restaurant/`

## Notes
- Images are pulled from Unsplash via URL for demo purposes — swap in your own photos by replacing the `src` attributes in `index.html`.
- The Google Map uses a generic embed URL; replace the address in the `iframe` `src` with your restaurant's real location.
