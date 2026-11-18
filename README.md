# Elin S. Hexspoor — portfolio website

Elin's personal portfolio: experience, education, awards, blog and contact.
Plain HTML, CSS and JavaScript. No build step and no framework.

- **Repository:** https://github.com/allcrumbs/elin-hexspoor
- **Live site:** https://allcrumbs.github.io/elin-hexspoor/ (GitHub Pages, published from `main`)

## Folders

```
index.html              home: intro, timeline, roles, expertise, contact
education.html          education
awards.html             awards list; one page per award in award/
blog.html               blog list; posts in blog/
contact.html            contact details and CV download
experience/             one page per role, linked from the home page
  _archive/             old role pages, not linked from the site
award/                  one page per award
blog/                   blog posts
css/styles.css          all styling; the copper colour is --accent at the top
js/main.js              timeline, accordion, fade-ins, copy-email buttons
assets/
  hero-bg.jpg           home page photo
  social-preview.jpg    1200x630 photo shown when the link is shared
  favicon.svg           browser tab icon
  cv/                   CV files; the site links to cv/Elin_Hexspoor_CV.pdf
  roles/                photos used on role and award pages
  _archive/             photos not used on the site
.nojekyll               tells GitHub Pages to serve files as they are
```

## Publishing

GitHub Pages publishes the `main` branch. Work on a branch, open a pull
request to `main`, and merge it; the site updates a minute or two later.

## Editing

- **Colour:** `--accent`, `--accent-deep` and `--accent-bright` at the top of `css/styles.css`.
- **Timeline:** the `<li class="era">` blocks in `index.html`.
- **Role list:** the `<a class="rcard">` blocks in `index.html`; each links to a page in `experience/`.
- **CV:** replace `assets/cv/Elin_Hexspoor_CV.pdf`, keeping the name.
- **Share preview:** `assets/social-preview.jpg` and the `og:` lines in `index.html`. The `og:image` and `og:url` lines hold the full site address; change them if the address changes.
- **Photos:** keep each under about 300 KB and no wider than 1400 px.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Open items

- `assets/cv/` holds four named CVs that are copies of the same file, and `assets/Elin_Hexspoor_CV.pdf` is an unused, different CV. To be replaced with the latest CV.
- Award descriptions on `awards.html` are best-guess context; check them.
