# CLAUDE.md

Elin's personal portfolio website. Plain HTML, CSS and JavaScript; no build step. See `README.md` for folders and publishing.

## Working with the owner

- The owner doesn't read code. Explain problems and changes in plain English, without jargon.

## Git

- Work on a branch and open a pull request to `main`. Merging to `main` publishes the site through GitHub Pages.
- Use Conventional Commits: imperative, lowercase, no trailing period, for example `fix(assets): shrink large photos`. Types: `feat`, `fix`, `docs`, `chore`, `refactor` (move or rename only), `design`. Scope is the top-level folder, when there is one.
- A commit message describes the change. Never quote or retell the chat.
- Move files with `git mv`, in commits apart from content edits.

## Keeping docs current

- Update `README.md` whenever pages, folders, file types, publishing or open items change.
- Update this file when the facts here change.

## Facts

- Live site: https://allcrumbs.github.io/elin-hexspoor/. The full address is also in the `og:image` and `og:url` lines of `index.html`.
- Pages people visit sit at the top level or in `awards/`, `blog/` and `experience/`. Everything else goes under `assets/`.
- Unused files go in the matching folder of `archive/`, not deleted. Pages there aren't kept working.
- The site shows Elin's previous official name nowhere. Keep it that way.
