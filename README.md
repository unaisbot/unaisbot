# unais.bot — The Alien Ecology (GitHub Pages migration starter)

This is a Jekyll starter for migrating `unaisbot.in` from Google Sites to GitHub Pages. It is designed to retain an editorial/nature-inspired identity while making articles easy to maintain as Markdown.

## Important: not the full content migration yet

The existing public homepage currently shows the site title/tagline and article titles including:
- Dark Diversity: The Hidden Side of Biodiversity
- Elysia chlorotica: The Solar-Powered Sea Slug
- The Science and Beauty of Iridescence

Those article bodies, original images, other pages, and their original URLs must be exported/collected from Google Sites before this starter can be considered a complete migration. Do not switch the live domain until that content is verified.

## Recommended repository

Use the GitHub account `unaisbot`. A repository named `blog` is suitable if you want the site at `blog.unaisbot.in`; for the root domain `unaisbot.in`, a repository named `unaisbot.github.io` is also suitable. The custom domain can be configured in GitHub Pages either way, but avoid using the same custom domain on multiple Pages sites.

## Add posts

Create a Markdown file under `_posts/` using the format `YYYY-MM-DD-title.md`, for example:

```markdown
---
layout: post
title: "Article title"
date: 2024-10-01
categories: [Biodiversity]
description: "A concise summary for cards and search engines."
image: /assets/images/article-cover.jpg
image_alt: "Descriptive text for the image"
permalink: /blog/article-title/
---

Paste the complete original article body here. Preserve headings, links, captions, references and image credits.
```

Place original images in `assets/images/`. Preserve credits and alt text. For every original page, record its old URL and the intended new permalink. Add redirects or matching permalinks where feasible.

## Google Sites migration checklist

1. Inventory every page and article in Google Sites, including embedded documents, galleries, external links, and downloads.
2. Copy/export full text and original media. Keep a local copy of the original site and assets.
3. Map every old URL to a new permalink; preserve paths where feasible.
4. Add all articles as `_posts/*.md`; add static pages as Markdown/HTML.
5. Check image ownership/credits and ensure no image URLs still depend on Google Sites.
6. Test desktop/mobile layout, navigation, accessibility, article links, and 404 handling.
7. Publish to a temporary `github.io` URL first.
8. Only after verification, set the custom domain in GitHub Pages and update GoDaddy DNS.
9. Keep the Google Sites version available until the new domain and all key pages are verified.

## GitHub Pages setup

- Upload the contents of this folder to the root of the selected repository.
- In **Settings → Pages**, configure deployment from the repository using GitHub Pages/Jekyll or GitHub Actions.
- Configure the custom domain only when ready to switch.
- This starter has `CNAME` set to `www.unaisbot.in`. If you choose `unaisbot.in` without `www`, change both `CNAME` and `_config.yml` `url` to `https://unaisbot.in`.
- Do not replace DNS records until the new Pages site is deployed and verified. GitHub's official custom-domain documentation should be followed for current DNS values.

## Notes

- The homepage includes a temporary stock forest hero image from Unsplash. Replace it with your original/approved banner if one exists.
- Some pages are marked as placeholders. Replace them with the original content before launch.
- `jekyll-feed` and `jekyll-seo-tag` are included through the GitHub Pages gem.
