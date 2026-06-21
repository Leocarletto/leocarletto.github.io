# leocarletto.github.io

Quarto website scaffold. Structure only — design/content to be added later.

## Build (dual language)

Main language is English (`index.qmd`); Portuguese is the toggle (`index.pt.qmd`).
Each page keeps both languages as sibling files inside the same folder.

```r
install.packages("babelquarto", repos = c("https://ropensci.r-universe.dev", "https://cloud.r-project.org"))
babelquarto::render_website(".")
```

Output goes to `docs/`. On GitHub: Settings → Pages → Source: `main` / `/docs`.
The EN/PT switch link is added to the navbar automatically by babelquarto.

## Structure

```
about/        About page (fixed bio, jolla template)
blog/         Blog listing + one folder per post
projects/     Projects landing (Publications + Packages)
  publications/   one folder per publication (EDA, model, experiment...)
  packages/       one folder per R package
```

Footer: GitHub + LinkedIn only.

## Why Publications is separate from Blog

Blog = short, informal notes/writing.
Publications = formal statistical deliverables (EDA, models, designed
experiments / t-tests) presented as portfolio pieces — each with a cover image,
grouped under Projects next to Packages, using a listing geared toward
analysis artifacts rather than chronological posts.
