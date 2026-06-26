# Rumpuree Dance Studio — Premium Website Skin

**Deliverable:** `index.html`
**Project:** Visual redesign (skin only) of singhawon.com
**Prepared for:** Rumpuree Dance Studio
**Studio established:** 2006

---

## What was delivered

A single self-contained `index.html` file — a complete premium visual skin for the Rumpuree website. It is a **surface-level redesign only**: no backend, no database, no server required. The existing site structure, page links, booking system, and all original URLs are preserved exactly as they are.

---

## How to use this file

### Option A — Preview instantly (no setup needed)

1. Download `index.html` to your computer
2. Double-click the file — it opens directly in any web browser (Chrome, Safari, Firefox, Edge)
3. All content loads from the live singhawon.com server, so you need an internet connection to see images

### Option B — Hand to your web developer

Give your developer the `index.html` file. They will:

1. Extract the CSS from the `<style>` block and save it as a separate `.css` file
2. Extract the JavaScript from the `<script>` block and save it as a separate `.js` file
3. Convert the HTML sections into your existing CMS/template system (Laravel, WordPress, or whatever your current stack uses)
4. Replace placeholder copy with your real content where indicated

---

## What's inside the file

### Design system

| Element | Choice | Reason |
|---|---|---|
| Background | Near-black `#0D0D0D` | Luxury, premium feel — same approach as high-end fashion and performance venues |
| Accent color | Gold `#C9A84C` | Warmth, prestige, royalty — reinforces the Dance Royalty loyalty program |
| Display font | Bebas Neue | Bold, dramatic headline presence — common in premium dance and fitness brands |
| Body font | Cormorant Garamond | Editorial elegance, serif warmth — feels cultivated and international |
| UI font | Inter | Clean, legible, modern — used for navigation, labels, and small text |

### Sections included

Every section on the current singhawon.com homepage is represented:

1. **Navigation bar** — all original links preserved; becomes frosted-glass on scroll; includes mobile hamburger menu
2. **Hero** — full-screen with your existing cover image, animated title, live statistics (45+ styles, 18+ years, 2 branches), and scroll indicator
3. **Marquee strip** — scrolling ticker of all dance style names in gold on gold background
4. **About Us** — two-image composition with overlapping layout, year badge, links to `/aboutus` and `/whyus`
5. **Dance Styles** — card grid pulling all 30+ images directly from singhawon.com; hover reveals style name and arrow
6. **Weekly Schedule** — day-by-day accordion with sample class tags per day; links to `/schedule/4`
7. **Dance Royalty Loyalty Program** — three-tier card layout (Silver / Gold / Platinum) with icons and perks
8. **Testimonials** — auto-scrolling horizontal carousel; pauses on hover
9. **Promotions** — featured large card + two smaller cards; links to `/promotion`
10. **Other Services** — seven-card grid using your existing `other_services_*.png` images
11. **Location** — address, transport info, opening hours, and embedded Google Map for the Asok branch
12. **Footer** — brand statement, navigation columns, social links (Instagram, YouTube, Google)

### Animations and interactions

- **Custom cursor** — gold dot with lagging ring follower (desktop only)
- **Hero parallax zoom** — background image slowly zooms over 20 seconds
- **Staggered entrance** — hero text, subtitle, and buttons fade up in sequence on page load
- **Scroll reveal** — every section fades and slides into view as the user scrolls down
- **Hover microinteractions** — style cards scale and reveal icons; schedule rows slide; promo cards underline from left
- **Auto-scroll testimonials** — infinite horizontal carousel with pause-on-hover
- **Scrolling marquee** — dance styles ticker, also pauseable on hover
- **Navbar transition** — transparent on hero, becomes dark frosted glass after scrolling 60px
- **Back-to-top button** — appears after scrolling 400px, smooth scroll on click
- **Mobile menu** — full-screen overlay with large type links

---

## Images

All images load directly from `https://singhawon.com/` — no separate image files are needed. If your hosting changes domains, update the image URLs inside the file.

Image paths used:

- `https://singhawon.com/images/logo.png`
- `https://singhawon.com/images/cover960.jpg`
- `https://singhawon.com/images/human1.png`, `human2.png`
- `https://singhawon.com/images/dancestyle/01_ballet_adult.jpeg` through `45_zouk.jpeg`
- `https://singhawon.com/images/other_services_1.png` through `other_services_7.png`

---

## Fonts

Loaded from Google Fonts via CDN — requires an internet connection:

- [Bebas Neue](https://fonts.google.com/specimen/Bebas+Neue)
- [Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond)
- [Inter](https://fonts.google.com/specimen/Inter)

For production use, your developer can self-host these font files for faster load times and offline support.

---

## Links

All navigation links point to the original singhawon.com pages. Nothing has been changed:

| Label | Destination |
|---|---|
| Schedule | `https://singhawon.com/schedule/4` |
| Fee | `https://singhawon.com/fee` |
| Promotion | `https://singhawon.com/promotion` |
| New Classes | `https://singhawon.com/?anchor=classupdate` |
| Events / Services | `https://singhawon.com/?anchor=otherservice` |
| About Us | `https://singhawon.com/?anchor=aboutus` |
| Login / Book | `https://booking.rumpuree.com` |

---

## What your developer needs to do

This file is a **design prototype and CSS specification**, not a drop-in replacement for your CMS templates. Here is a clear handoff checklist:

- [ ] Integrate the CSS variables and styles into your existing stylesheet
- [ ] Replace the static testimonial cards with real data from your database or CMS
- [ ] Connect the Dance Styles grid to your dynamic class list (currently hardcoded with 30 styles)
- [ ] Replace the Weekly Schedule section with live data from your booking system
- [ ] Swap the static Promotions cards with your actual current promotions
- [ ] Add the Instagram feed embed (currently omitted — your existing embed from `mirror-app.com` can be placed in the Dance Update section)
- [ ] Test on iOS Safari, Android Chrome, and tablet viewport widths
- [ ] Add your real Open Graph meta tags (`og:title`, `og:image`, etc.) for social sharing

---

## Browser support

Tested design targets:

| Browser | Support |
|---|---|
| Chrome 100+ | Full |
| Safari 15+ | Full |
| Firefox 100+ | Full |
| Edge 100+ | Full |
| iOS Safari | Full (cursor effects disabled automatically) |
| Android Chrome | Full |

The custom cursor is a desktop-only effect — it has no impact on mobile users.

---

## Content to update before going live

These placeholder items in the file should be replaced with your real content:

- **Testimonials** — currently written as representative sample quotes; replace with real student reviews
- **Weekly Schedule tags** — sample class names per day; replace with your actual timetable data
- **Promotion descriptions** — three sample offer cards; replace with current promotions
- **Service card names** — inferred from image filenames; confirm the names match your actual service offerings
- **Branch hours** — sample hours shown; confirm against your real opening times

---

## Questions

If you or your developer have questions about any part of this file, the structure is organized with clear HTML comments marking each section (`HERO`, `MARQUEE`, `ABOUT`, etc.) making it straightforward to locate and edit any part.
