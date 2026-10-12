# Website maintenance

A single-page professional website at [jadeohlhauser.com](https://jadeohlhauser.com/), hosted with GitHub Pages from the root of `main`.

The site is plain HTML and CSS, with no build step or JavaScript dependencies. The root `README.md` appears on the public GitHub profile and contains the professional introduction; keep maintenance information in this file.

## Local preview

Run from this folder:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open [http://127.0.0.1:8000](http://127.0.0.1:8000). Refresh the browser after changes.

## Visual assets

The portrait and original JTS logo in `assets/` are copied from the JTS website source. The palette uses olive charcoal (`#34362b`), warm white (`#f3f3ec`), and soft mint (`#c3e7cc`).

The favicon is a JO monogram in olive and mint. `assets/favicon.svg` is the editable source; `jade-icon.png` is the PNG fallback.

## LinkedIn banner

Upload `assets/linkedin-banner.png` as the personal profile's cover image. It is 1584 × 396 pixels. `assets/linkedin-banner.svg` is the editable source: an olive background with subtle geometric linework and no text.

## JTS domain

Cloudflare redirects `jts.ltd` and `www.jts.ltd`, including all paths, to `https://jadeohlhauser.com/` with a 301 permanent redirect. The redirect rule is named **JTS website redirect**.

Cloudflare also hosts the DNS records for Microsoft 365 email on `jts.ltd`. Preserve the existing email records when making website changes.
