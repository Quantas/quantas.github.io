# website

Source for [www.quantasnet.com](https://www.quantasnet.com), Andrew Landsverk's home page.

Plain HTML and CSS in `site/`, with no build step and no dependencies.

- Preview: `python3 -m http.server -d site 8000`, then open http://localhost:8000
- Test: `python3 -I -m unittest discover -s tests -v`
- Deploy: every push to `main` publishes `site/` to GitHub Pages (`.github/workflows/ci.yml`).

This is the `Quantas` user site, so GitHub serves every `Quantas` project Pages site under the same domain, at `www.quantasnet.com/<repo>/`. Don't add a top-level directory named after a project repo; it would compete with that project's site.

The exception is a project that moved away: its old path gets a redirect page, so existing links keep working. `site/shark-ng-table/` sends visitors to https://shark-ng-table.sharkops.io/, keeping the `#/...` part of the URL.

Licensed under Apache-2.0.
