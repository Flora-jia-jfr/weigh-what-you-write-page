# Weigh what you write: proposal page

A one-page site for the research proposal *Do reasoning models weigh what they write? Verbalization and the use of parametric priors under test-time compute* (proposal v2, 2026-10-29). Its layout follows the group's [step-back page](https://flora-jia-jfr.github.io/step-back-page/).

This repo holds only the frontend. Code, data and the full proposal (in Chinese) live in the separate experiment repo, `weigh-what-you-write`.

## Files

- `index.html`: the whole page, with its styles and the script that draws the figures. There is no build step; the only outside dependency is Google Fonts.
- `.nojekyll`: tells GitHub Pages to serve the files unchanged.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Publish with GitHub Pages

Settings → Pages → Build and deployment → Deploy from a branch → `main`, `/ (root)`. The site then appears at `https://<owner>.github.io/weigh-what-you-write-page/`. On a free GitHub plan, Pages needs a public repo.

## What to update

- `CODE_REPO`, at the top of the script in `index.html`: set it to the experiment repo's URL. The "Code & data", "Pilot design" and "Full proposal" links stay hidden while it is empty.
- `<meta name="robots" content="noindex, nofollow">`: keeps the unpublished proposal out of search results. Remove it once the paper is public.
- When pilot results arrive, replace the empty frame in Figure 3 and the footer line "No model has been run".
