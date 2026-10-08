# Wu-Tang Clan Site

A multi-page site for the Wu-Tang Clan: a homepage with a hover-reveal hero image, a dropdown-nav member directory (10 bio pages), two album pages, and an embedded browser game.

**Live site:** https://YOUR-USERNAME.github.io/wu-tang-clan-website/

## What this is

One of my first web projects — originally built for an intro web design course:

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

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server
```

## Deploying

This is ready for GitHub Pages: push this folder to a repo, then in **Settings → Pages** set the source to the root of the `main` branch. `index.html` will be served automatically.

