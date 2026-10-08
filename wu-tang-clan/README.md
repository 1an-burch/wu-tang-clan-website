# Wu-Tang Clan Fan Site

A multi-page fan site for the Wu-Tang Clan: a homepage with a hover-reveal hero image, a dropdown-nav member directory (10 bio pages), two album pages, and an embedded browser game.

## What this is

One of my first web projects — originally built for an intro web design course. This version has been cleaned up from the original coursework submission:

- **Consolidated CSS**: the same ~100-line `<style>` block used to be copy-pasted into all 14 HTML files. It now lives in one shared `styles.css`.
- **Fixed invalid HTML**: the original had duplicate `<body>` tags and a `<style>` block placed after `</body>` on every page. Every page now has valid structure (`doctype`, single `head`/`body`, proper nesting).
- **Fixed a real bug**: the logo image was referenced as `logoimage.png` but saved as `logoimage.PNG`. That works on Windows/Mac (case-insensitive file systems) but silently breaks on GitHub Pages / Linux. Fixed.
- **Cleaner filenames & URLs**: pages are no longer numbered (`1rza.html` → `rza.html`), and the homepage is `index.html` so it works as a proper site root.
- **Better accessibility**: replaced placeholder alt text (`alt="pls"`, `alt="u god??"`) with real descriptions.
- **Small responsive tweak**: bio pages now stack on narrow screens instead of only working at desktop width.

The content and design (layout, colors, hover effects, nav structure) are unchanged — this is a structural cleanup, not a redesign.

## Structure

```
├── index.html
├── styles.css
├── rza.html, gza.html, ... (10 member bio pages)
├── enter-the-wu-tang.html, wu-tang-forever.html (album pages)
├── wu-tang-shaolin-style.html (game page)
└── images/
```

## Running it locally

No build step — it's static HTML/CSS. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server
```

## Deploying

This is ready for GitHub Pages: push this folder to a repo, then in **Settings → Pages** set the source to the root of the `main` branch. `index.html` will be served automatically/