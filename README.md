# website

Source for [www.quantasnet.com](https://www.quantasnet.com), Andrew Landsverk's home page.

Plain HTML and CSS in `site/`, with no build step and no dependencies.

- Preview: `python3 -m http.server -d site 8000`, then open http://localhost:8000
- Test: `python3 -I -m unittest discover -s tests -v`
- Deploy: every push to `main` publishes `site/` to GitHub Pages (`.github/workflows/ci.yml`).

`site/shark-ng-table/` redirects the old demo URL to `https://quantas.github.io/shark-ng-table/`.

Licensed under Apache-2.0.
