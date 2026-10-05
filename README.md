# Corey Italiano — Author Website

Official website for science fiction author **Corey Italiano**, featuring the Dova Sku Series and companion app. Built with plain HTML and CSS — no frameworks, no build tools, no dependencies.

**Live site:** [coreyitaliano.com](https://coreyitaliano.com)

---

## Pages

| File | Description |
|---|---|
| `index.html` | Home page — hero, companion app section, about, series, future projects, newsletter |
| `books.html` | Full bibliography — Transync, Ascendant, Book 3 placeholder, standalones |
| `universe.html` | Dova Sku universe lore and world-building |
| `sample.html` | Free sample read |
| `privacy.html` | Privacy policy |

---

## Project Structure

```
/
├── index.html
├── books.html
├── universe.html
├── sample.html
├── privacy.html
└── images/
    ├── App-website-background.png   # Full-page background image (all pages)
    ├── TransyncFrontV2.jpg          # Transync cover (hero + cards)
    ├── TransyncCoverV2.png          # Transync cover (books page)
    ├── AscendantCover.png           # Ascendant cover (hero + cards)
    ├── ascendant-cover.jpg          # Ascendant cover (books page)
    ├── ComingSoon.jpg               # Book 3 placeholder cover
    ├── headshot.png                 # Author photo
    ├── Logo.png                     # Corey Italiano logo (footer strip)
    ├── app1.jpg                     # Companion app screenshot 1
    ├── appT.jpg                     # Companion app screenshot 2
    ├── app3.jpg                     # Companion app screenshot 3
    └── app4.jpg                     # Companion app screenshot 4
```

---

## Design System

All pages share a consistent set of CSS custom properties defined in `:root`:

| Variable | Value | Usage |
|---|---|---|
| `--accent` | `#ff6b2c` | Orange — primary buttons, highlights |
| `--accent-soft` | `#f59e0b` | Amber — kicker labels, links |
| `--ink` | `#f9fafb` | Primary text |
| `--ink-muted` | `#9ca3af` | Secondary text, descriptions |
| `--card-radius` | `1rem` | Card border radius |
| `--max-width` | `1100px` | Page content max width |

**Background:** A full-viewport image (`App-website-background.png`) with a dark gradient overlay (`rgba(0,0,0,0.65)` to `rgba(0,0,0,0.75)`). Background position is set to `left center` to keep the focal figure on the right side of the screen. On mobile, `background-attachment` switches from `fixed` to `scroll` to fix an iOS Safari rendering bug.

---

## Key Sections (index.html)

### Hero
Dual book cover stack with CSS `rotate` transforms and hover animation. Buttons link to Amazon, Barnes & Noble, and internal pages.

### Companion App
Four app screenshots displayed in a 4-column grid, followed by the section title, description, and store buttons.

- App Store: [The Dova Sku Series Companion](https://apps.apple.com/app/the-dova-sku-series-companion/id6761311290)
- Google Play: [The Dova Sku Series Companion](https://play.google.com/store/apps/details?id=com.coreyitaliano.bookcompanion)

### About
Author bio with headshot photo. Paired with the Series card in a two-column grid.

### Series
Overview of the Dova Sku Series with book cards for Transync and Ascendant linking to `books.html`.

### Future Projects
Book 3 teaser and call to join the mailing list.

### Newsletter
Email signup form. Currently uses `mailto:` as a placeholder — replace the `action` attribute with a Mailchimp or ConvertKit embed URL when ready.

---

## Fixes & Notes

- `background-attachment: scroll` is applied on mobile via media query to fix an iOS Safari rendering bug with `fixed` backgrounds (applied to all pages)
- All below-fold images use `loading="lazy"` for performance
- Open Graph and Twitter Card meta tags are present on `index.html` for social sharing previews
- The nav brand on sub-pages (`books.html`, `privacy.html`) links back to `index.html` as an `<a>` tag rather than a plain `<div>`
- `books.html` has proper closing tags for all `<section>` and `<div>` elements

---

## Contact & Social

| Platform | Link |
|---|---|
| Email | imaginariumitaliano@gmail.com |
| Amazon | [Author Page](https://www.amazon.com/stores/Corey-Italiano/author/B0CZJZ7DSH) |
| Barnes & Noble | [Author Page](https://www.barnesandnoble.com/s/%22Corey%20Italiano%22) |
| Facebook | [Imaginariumitaliano](https://www.facebook.com/Imaginariumitaliano) |
| Instagram | [@coreyitaliano.author](https://www.instagram.com/coreyitaliano.author/) |
| TikTok | [@paisanitaliano](https://www.tiktok.com/@paisanitaliano) |
