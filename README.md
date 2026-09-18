# Razed Barber & Beauty — Website

A modern, dark, single-page site for Razed Barber & Beauty (Jonesboro, GA). Plain HTML/CSS/JS — no build step, no framework — so it deploys on Vercel as a static site with zero configuration.

## Structure

```
index.html        Page markup (Hero, About, Services, Gallery, Contact, Footer)
css/style.css      All styling, layout, and animations
js/main.js         Scroll reveal, nav, mobile menu, lightbox, parallax, cursor
images/            Logo, favicons, and shop photos
```

## Run locally

Any static server works, e.g.:

```
npx serve .
# or
python3 -m http.server 8080
```

## Deploy to Vercel

Push this folder to GitHub and import it in Vercel — no framework preset or build command needed ("Other" / static). Vercel will serve `index.html` at the root automatically.

## ⚠️ Please verify before publishing

The contact details below were pulled from public directory listings (Fresha, Yellow Pages) since they weren't provided directly — please confirm they're current:

- **Address:** 7868 Tara Blvd, Jonesboro, GA 30236
- **Phone:** (678) 586-3200
- **Hours:** Mon–Sat 10:00 AM–8:00 PM, Sun 10:00 AM–3:00 PM (two directories disagreed slightly on Saturday/Sunday hours — worth double-checking)
- **Facebook:** facebook.com/razedbarberandbeautysalon

Also worth adding once you have them: an Instagram link, and real pricing if you'd like it listed under Services (currently omitted since it wasn't confirmed).

## Customizing

- Colors, fonts, spacing: top of `css/style.css` under `:root`.
- Copy/text: edit directly in `index.html`.
- Photos: swap files in `images/` (keep the same filenames, or update the `src`/`data-full` attributes in `index.html`).
- "Book Now" currently calls the shop (no online booking platform configured). If you add one (Booksy, Square, Vagaro, etc.), point the `.btn--solid` "Book Now" links and the `#contact` CTA at that link instead of `tel:`.
