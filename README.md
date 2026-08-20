# Stokky — site

Public hosting for the Stokky landing page, kept separate from the app
repository so the source code stays private.

- [Landing page](https://andryhenintsoa.github.io/stokky-site/) — `index.html`

The page is self-contained: fonts are self-hosted, icons are inline SVG, and it
makes no external request at all — no CDN, no Google Fonts, no analytics.

## Updating

The source of truth lives in the app repository at `docs/site/`. Edit there,
then copy over and push:

```bash
cp -R ../stokky/docs/site/index.html ../stokky/docs/site/assets .
git commit -am "docs: sync the landing page" && git push
```
