# Reza Emrani website skeleton

Bilingual Persian/English author and linguist website.

## Stack

- GitHub repository: source and history
- GitHub Pages: public hosting
- Jekyll: static site generator supported natively by GitHub Pages
- Pages CMS: browser-based editing for nontechnical collaborators
- Custom domain: intended for `rezaemrani.com`

## Structure

- `/en/` English website
- `/fa/` Persian website
- `_books_en/`, `_books_fa/` book records
- `_publications_en/`, `_publications_fa/` article/publication records
- `assets/images/` images and book covers
- `assets/documents/` PDFs
- `.pages.yml` Pages CMS configuration

## First deployment

1. Create a GitHub repository, e.g. `rezaemrani-site`.
2. Upload all files in this folder to the repository root.
3. In GitHub: Settings → Pages.
4. Set source to "Deploy from a branch", branch `main`, folder `/ (root)`.
5. Wait for the default `github.io` site to publish.
6. Open Pages CMS, connect the repository, and confirm the editable sections appear.

## Custom domain

Do not add the custom domain until the domain is actually registered.

After registering `rezaemrani.com`:

1. Add `rezaemrani.com` under GitHub → Settings → Pages → Custom domain.
2. Configure the registrar's DNS records using GitHub's current custom-domain instructions.
3. Also configure `www.rezaemrani.com`.
4. Enable HTTPS in GitHub Pages once DNS has propagated.

`CNAME.example` is included only as a reminder. It should not be renamed to `CNAME` until the domain is ready.

## Editing

Editors should use Pages CMS, not GitHub.

They can:
- edit English and Persian biographies/contact pages
- add/edit books
- add/edit publications
- upload images
- upload PDFs

Site templates, layout, CSS, RTL behavior, and navigation stay outside the normal editorial interface.
