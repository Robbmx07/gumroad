# robbmx landing page

Static single-file landing page for robbmx's Gumroad store (`robbmx.gumroad.com`). Links out to both products and embeds a Gumroad "Follow" form to collect emails.

## Deploy with GitHub Pages

1. In this repo: Settings → Pages → Deploy from branch → pick this branch, folder `/ (root)`.
2. GitHub serves `index.html` at `https://<your-username>.github.io/<repo>/`.
3. Optional: add a custom domain under Settings → Pages → Custom domain (e.g. `robbmx.com`), and point that domain's DNS at GitHub Pages.

## Why not just paste this into Gumroad's own profile editor

Gumroad's native profile page (`gumroad.com/robbmx`) is built from its own theme/sections system and doesn't accept raw custom HTML/CSS — so this page is meant to be hosted on your own domain (or GitHub Pages) as your "home base," with buttons linking into your actual Gumroad product pages. That's also why the Follow form needs Gumroad's embed script (`https://gumroad.com/js/gumroad.js`), which was added at the bottom of `index.html` — without it the `data-gumroad-follow` form doesn't submit.
