# piketremor.github.io

Quarto website for Mike Premer's software and publications. Deployed to GitHub Pages by GitHub Actions on every push to `main`.

## One-time setup
1. Create an **empty public** repo named exactly `piketremor.github.io` on GitHub.
2. From this folder:
   ```
   git init -b main && git add . && git commit -m "Initial site"
   git remote add origin https://github.com/piketremor/piketremor.github.io.git
   git push -u origin main
   ```
3. Wait for the "Publish site" action to finish (creates the `gh-pages` branch).
4. Repo → Settings → Pages → Source: *Deploy from a branch* → `gh-pages` / `(root)`.
5. Site goes live at https://piketremor.github.io.

## Editing
- `index.qmd` home · `software.qmd` featured + auto-listed repos · `publications.qmd` + `publications.bib`
- Add papers: paste BibTeX into `publications.bib`.
- Preview locally: `quarto preview`
- Custom domain later (e.g. maineforestlab.com): add a `CNAME` file containing the domain and list it under `project: resources:` in `_quarto.yml`, then point DNS at GitHub Pages.
