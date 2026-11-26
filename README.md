# Wealth Angels website

The one-page website for **Wealth Angels**, the financial-education community led by Sonny Kirtley and Diego Taira.

It's a single static page with no build step: plain HTML, CSS and a little JavaScript.

```
index.html      the whole page (markup, styles and scripts)
favicon.ico     browser-tab icon (16, 32 and 48px)
assets/         the logo, photos and app icons
```

The favicon and app icons (`assets/favicon-32.png`, `apple-touch-icon.png`, `icon-192.png`) use the wings from the logo, in white on Night Navy.

`assets/social-preview.jpg` (1200×630) is the image shown when the link is shared on Facebook, LinkedIn, X, WhatsApp and iMessage. The sharing tags in `index.html` point to `https://wealth-angels.com/`; if the site goes live at a different address, update the `og:url`, `og:image`, `twitter:image` and `canonical` tags to match.

## Preview locally

Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

then visit http://localhost:8000.

## Hosting

Any static host works. Point it at the repo root with no build command:

- **Vercel / Netlify / Cloudflare Pages:** import the repo, leave the build command empty, output directory `/`.
- **GitHub Pages:** Settings → Pages → deploy from the `main` branch, root folder.

## Fonts

Loaded from Google Fonts:

- **Archivo** for headlines, labels and buttons, at its widest width (`wdth` 125) and weights 700–800. Keep the `wdth` axis in the font URL, or the headlines lose their wide shape.
- **Montserrat** (400, 500, 600) for body text.

## Motion

Reveal-on-scroll, word-by-word headings, the growing tree in the hero, hover lifts and the count-up are all in the script at the bottom of `index.html`. Visitors whose device is set to reduce motion get the finished page with no animation.

## Before launch

- Join buttons point to `https://community.wealth-angels.com`. Confirm that's the right link.
- Mastering Money is described as a "monthly membership" with no price shown.
- The Options for Investors course page on Maven currently says the course is no longer available.

Prepared by Block Ten Strategy.
