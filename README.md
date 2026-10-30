# Weigh what you write: proposal page

A one-page public site for the research proposal *Do reasoning models weigh what they write? Verbalization and the use of parametric priors under test-time compute*: <https://flora-jia-jfr.github.io/weigh-what-you-write-page/>. Its layout follows the group's [step-back page](https://flora-jia-jfr.github.io/step-back-page/).

## What goes on the page

The page is public, so it carries only the proposal's research content: the question, motivation and related work, research questions, and the experiment design. Project management stays out: timelines, compute budgets, risks, stopping rules, venue plans, internal decisions, and unpublished results. Every plot is a schematic.

The design shown here mirrors the plan in the private code-and-data repo (`weigh-what-you-write`, file `PLAN.md`). When a design decision there changes, update this page to match.

## Files

- `index.html`: the whole page, with its styles and the script that draws the figures. There is no build step; the only outside dependency is Google Fonts.
- `.nojekyll`: tells GitHub Pages to serve the files unchanged.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Publishing

GitHub Pages serves `main` from the repo root. A push to `main` goes live in about 90 seconds.

The page has `<meta name="robots" content="noindex, nofollow">` because the work is unpublished. Remove it once the paper is public.
