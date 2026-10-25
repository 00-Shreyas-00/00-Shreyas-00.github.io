# 00-Shreyas-00.github.io

Personal portfolio of Shreyas Shinde, built from the "Portfolio UI – Web & Mobile" Figma community template with [Eleventy](https://www.11ty.dev/) and deployed to GitHub Pages.

## Develop

```bash
npm install
npm start        # http://localhost:8080
npm run build    # static output in _site/
```

## Editing content

| What | Where |
| --- | --- |
| Name, intro, links, email | `src/_data/site.json` |
| Projects (Work + detail pages) | `src/works/*.md` — `featured: true` puts one on Home, `order` sets position, `image` adds a thumbnail |
| Blog posts | add `src/blog/posts/my-post.md` (see below); "Recent posts" on Home appears automatically |
| Résumé / photo | `src/assets/` |
| Styles | `src/assets/css/style.css` |

Blog post front matter:

```md
---
title: My first post
date: 2026-11-01
topics: Go, Kubernetes
summary: One or two sentences shown in the listing.
---
Post body in Markdown.
```

Project images: put a file in `src/assets/img/works/` and add `image: /assets/img/works/cleanzy.png` (thumbnail, 246×180 crop) to the project's front matter. The same image appears full-width on the detail page; add more with Markdown `![alt](/assets/img/works/...)` in the body.

## Deploy

Pushing to `main` runs `.github/workflows/deploy.yml`, which builds the site and publishes `_site/` to GitHub Pages. In the repository settings, **Pages → Build and deployment → Source** must be set to **GitHub Actions**.
