# Floral Fromage — landing page

A single-page "we'll be back soon" landing page for [Floral Fromage](https://www.floralfromage.com),
a dried flowers & artisanal cheese shop in Brooklyn, NY, while the main site is being renovated.

Static HTML/CSS — no build step. Hosted on GitHub Pages.

## Structure

```
index.html      # the page
styles.css      # all styling
assets/
  logo-mark.png # circular monogram logo
  favicon.png   # browser tab icon
  photos/       # gallery images
```

## Develop locally

Just open `index.html` in a browser, or serve it:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Editing content

- **Contact details, message text, links** — edit `index.html`.
- **Colors, fonts, spacing** — edit the `:root` variables at the top of `styles.css`.
- **Instagram gallery (optional)** — the `<section id="instagram">` in `index.html`
  embeds specific Instagram posts via Instagram's official `embed.js`. To change which
  posts show, edit the `data-instgrm-permalink` URLs in the `.ig-embeds` block (one
  `<blockquote class="instagram-media">` per post). The section **auto-hides** if the
  embeds don't load, and can be removed entirely by deleting the `<section>`.

## Credits

- Fonts: [Fraunces](https://fonts.google.com/specimen/Fraunces) +
  [Mulish](https://fonts.google.com/specimen/Mulish) via Google Fonts.
- Photography: Floral Fromage.
