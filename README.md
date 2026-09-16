# ForgeDITA Website

This repository contains the static website for [forgedita.com](https://www.forgedita.com).

## Site structure

- `index.html`: product landing page
- `architecture.html`, `conformance.html`, `status.html`, `about.html`: product evidence and project context
- `blog/`: published article pages and the blog index
- `content/blog/`: Markdown source for the 24-article editorial plan
- `*-alternative.html`: comparison and evaluation pages
- `rss.xml`, `sitemap.xml`, `robots.txt`: discovery files
- `styles.css`: shared site styling

## Preview locally

From the repository root, run:

```powershell
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Publishing an article

The first six articles in `content/blog/` are published as HTML in `blog/`. The remaining 18 are complete drafts. To publish one:

1. Review its Markdown source and change `status: draft` to `status: published`.
2. Add the publication date.
3. Create the corresponding HTML page using an existing article page as the template.
4. Add its card to `blog/index.html`.
5. Add it to `rss.xml` and `sitemap.xml`.
6. Check navigation, metadata, and responsive layout before deployment.

The site is intentionally dependency-free and can be hosted directly with GitHub Pages.
