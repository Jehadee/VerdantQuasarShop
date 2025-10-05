# VerdantQuasar – Houseplants Shop

A simple, responsive 3-page storefront built with plain HTML, CSS, and JavaScript. It includes a landing page, product listing with categories and Add to Cart, and a shopping cart with quantity controls, totals, and basic navigation.

## Author
- Creator: Jehadee L. Macadato

## Pages
- Landing: `index.html` – background image, brand, company blurb, Get Started.
- Products: `products.html` – 6 plants in 3 categories, thumbnails, name, price, Add to Cart.
- Cart: `cart.html` – item list with image/name/price, increase/decrease/delete, totals, checkout alert, continue shopping (top and bottom).

## Features
- Shared header with cart icon and live count across pages.
- Add to Cart: increments count, disables button, persists to `localStorage`.
- Cart controls: increment/decrement/delete per item, recalculates totals.
- Responsive layout for mobile (768px and 480px breakpoints).
- Hover effects for product cards and buttons.
- Redux-style store for cart state with actions (ADD, INC, DEC, DEL).

## Tech
- No frameworks; just static assets.
- Redux-style store in `js/store.js` (tiny createStore, reducer, actions).
- State persistence via `localStorage` under key `verdantquasar_cart_v1`.

## Folder structure
```
  index.html
  products.html
  cart.html
  css/
    styles.css
  js/
    scripts.js
    store.js
  images/
    Assorted Succulent.avif
    Calathea.webp
    Golden Pothos.jpg
    Parlor Palm.jpg
    Snake Plant.jpg
    ZZ Plant.jpg
  README.md
```

## How to run locally
- Option 1: Open `index.html` directly in a browser.
- Option 2 (recommended for Chrome file:// restrictions): serve the folder with a simple server.
  - Python 3: `python -m http.server 8000` then visit `http://localhost:8000//index.html`.

## Live demo (GitHub Pages)
Enable GitHub Pages (Settings → Pages → Build and deployment: Deploy from a branch → Branch: `main` → `/root`). Then use:

- Landing: https://github.com/Jehadee/VerdantQuasarShop.git/index.html
- Products: https://github.com/Jehadee/VerdantQuasarShop.git/products.html
- Cart: https://github.com/Jehadee/VerdantQuasarShop.git/cart.html

Repo: https://github.com/Jehadee/VerdantQuasarShop

## Customization
- Brand name is `VerdantQuasar` (change in all HTML titles/headers if you want).
- Images live in `images/`; product cards reference files by exact filename.
- To reset the cart, clear browser storage for this site or change `STORAGE_KEY` in `js/scripts.js`.

## Grading checklist mapping (for instructors)
- Landing page: background, paragraph, company name, CTA to products.
- Product listing: 6 unique plants, 3 categories, Add to Cart disables + increments + persists.
- Header: appears on products/cart, cart icon shows total items, nav between pages.
- Cart: total items, total cost, per-item thumbnail/name/unit price, increase/decrease/delete, checkout alert, continue shopping top and bottom.


