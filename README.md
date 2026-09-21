# Reza Emrani website

Bilingual Persian/English author and linguist website.

## Current preview

https://sepante.github.io/rezaemrani/

## Design

Yellow, minimal, large-type editorial design inspired by the general visual direction of Wynn:
bright monochrome colour, oversized typography, strict rules, and very little ornament.

No external web fonts are required, which also avoids depending on a font CDN for visitors in Iran.

## Current routing

The two critical language pages are real files:

- `en/index.html` → `/rezaemrani/en/`
- `fa/index.html` → `/rezaemrani/fa/`

Navigation within each language uses page anchors (`#about`, `#books`, etc.), reducing the number
of routes that can break while the site is still small.

## GitHub Pages

Current `_config.yml`:

```yaml
url: "https://sepante.github.io"
baseurl: "/rezaemrani"
```

When `rezaemrani.com` is connected, change that to:

```yaml
url: "https://rezaemrani.com"
baseurl: ""
```

## Pages CMS

`.pages.yml` exposes:

- English home-page text
- Persian home-page text
- English/Persian books
- English/Persian publications
- image uploads
- PDF uploads

The layout and CSS are not part of the normal editing interface.

## Uploading this version

Replace the existing site files in the repository root with the contents of this ZIP.
Do not upload the ZIP itself as a single file.
