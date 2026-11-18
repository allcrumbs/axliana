# Elin S. Hexspoor — portfolio website

Elin's personal portfolio: experience, education, awards, blog and contact.
Plain HTML, CSS and JavaScript. No build step and no framework.

- **Repository:** https://github.com/allcrumbs/elin-hexspoor
- **Live site:** https://allcrumbs.github.io/elin-hexspoor/ (GitHub Pages, published from `main`)

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
  cv/                   CV files; the site links to Elin_Hexspoor_CV.pdf
archive/                unused files, kept for reference, not linked from the site
  experience/           old role pages
  images/               old photos
  cv/                   old CV
.nojekyll               tells GitHub Pages to serve files as they are
```

## Publishing

GitHub Pages publishes the `main` branch. Work on a branch, open a pull
request to `main`, and merge it; the site updates a minute or two later.

## Editing

- **Colour:** the green `--accent`, `--accent-deep` and `--accent-bright` at the top of `assets/css/styles.css`.
- **Timeline:** the `<li class="era">` blocks in `index.html`.
- **Role list:** the `<a class="rcard">` blocks in `index.html`; each links to a page in `experience/`.
- **CV:** replace `assets/cv/Elin_Hexspoor_CV.pdf`, keeping the name.
- **Share preview:** `assets/images/social-preview.jpg` and the `og:` lines in `index.html`. The `og:image` and `og:url` lines hold the full site address; change them if the address changes.
- **Photos:** put them in `assets/images/photos/`; keep each under about 300 KB and no wider than 1400 px.
- **Unused files:** move them to the matching folder in `archive/` rather than deleting them.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Open items

- `assets/cv/` holds four named CVs that are copies of the same file the site links to. To be replaced with the latest CV.
- Award descriptions on `awards.html` are best-guess context; check them.
