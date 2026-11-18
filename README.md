# Elin S. Hexspoor — portfolio website

Elin's personal portfolio: experience, education, awards, blog and contact.
Plain HTML, CSS and JavaScript. No build step and no framework.

- **Repository:** https://github.com/allcrumbs/axliana
- **Live site:** https://axliana.com (GitHub Pages, published from `main`)

## Folders

```
index.html              home: intro, timeline, roles, expertise, contact
education.html          education
awards.html             awards list
blog.html               blog list
contact.html            contact details and CV download
awards/                 one page per award
blog/                   one page per blog post
experience/             one page per role, linked from the home page
assets/                 everything that isn't a page
  css/styles.css        all styling; the green accent colour is --accent at the top
  js/main.js            timeline, accordion, fade-ins, copy-email buttons
  images/
    hero-bg.jpg         home page photo
    social-preview.jpg  1200x630 photo shown when the link is shared
    favicon.svg         browser tab icon
    photos/             photos used on role and award pages
  cv/Elin_Hexspoor_CV.pdf  the CV the site links to
archive/                unused files, kept for reference, not linked from the site
  experience/           old role pages
  images/               old photos
  cv/                   old CVs
CNAME                   the site's domain, axliana.com, for GitHub Pages
.nojekyll               tells GitHub Pages to serve files as they are
LICENSE                 copyright notice: all rights reserved
```

## Publishing

GitHub Pages publishes the `main` branch at axliana.com. Work on a branch,
open a pull request to `main`, and merge it; the site updates a minute or
two later.

The domain is registered at Neoserv. Its DNS points at GitHub Pages:
four `A` records for `axliana.com` (185.199.108.153, 185.199.109.153,
185.199.110.153, 185.199.111.153) and a `CNAME` record for `www` to
`allcrumbs.github.io`. To move to another host, change these records and
the `CNAME` file; the address stays the same.

## Editing

- **Colour:** the green `--accent`, `--accent-deep` and `--accent-bright` at the top of `assets/css/styles.css`.
- **Timeline:** the `<li class="era">` blocks in `index.html`.
- **Role list:** the `<a class="rcard">` blocks in `index.html`; each links to a page in `experience/`.
- **CV:** replace `assets/cv/Elin_Hexspoor_CV.pdf`, keeping the name. Leave out the street address.
- **Share preview:** `assets/images/social-preview.jpg` and the `og:` lines in `index.html`. The `og:image` and `og:url` lines hold the full site address; change them if the address changes.
- **Photos:** put them in `assets/images/photos/`; keep each under about 300 KB and no wider than 1400 px. Galleries use `<div class="photo-grid">` and show each photo whole.
- **Unused files:** move them to the matching folder in `archive/` rather than deleting them.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Copyright

© 2026 Elin S. Hexspoor. All rights reserved. The code, design, text and
photos may not be copied or reused without written permission. See `LICENSE`.

## Open items

- Award descriptions on `awards.html` are best-guess context; check them.
