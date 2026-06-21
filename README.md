# leocarletto.github.io

Personal Quarto website. Pages: Posts (home), Gallery, Projects, About (EN/PT/ES).
Font: Cascadia Code. Theme: orange. Pure markdown — rendering needs only Quarto.

## IMPORTANT: put your photo as `logo.png`
Place your GitHub profile photo as `logo.png` in the project root.
It is used as: navbar logo, browser-tab favicon, and the About page photo.
(This file is intentionally NOT in the archive so it never overwrites yours.)

## Build & deploy
```bash
quarto render
git add -A
git commit -m "update site"
git push
```
GitHub → Settings → Pages → Deploy from a branch → main / docs.

## Structure
```
index.qmd                  Posts listing (home)
posts/<post>/index.qmd     one folder per post
gallery/index.qmd          Quarto Gallery page
projects/index.qmd         Projects listing (cards)
projects/eda-inmetro/      EDA project page (capa.jpg + Website/Repository buttons)
about/index.qmd            About EN  (photo + intro + latest projects)
about/index.pt.qmd         About PT
about/index.es.qmd         About ES
styles.scss                Cascadia Code + orange theme
tomorrow-night-bright-r-classic.theme   code highlight
logo.png                   YOUR photo (add it yourself)
```
