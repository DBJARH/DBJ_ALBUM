# CLAUDE.md

This file is written for Claude. It describes this repository and how Claude should behave here.

## What This Repo Is

**DBJ_ALBUM** is DBJ's public album — a mixed media portfolio (images and writeups).

- Live site: https://DBJARH.github.io/DBJ_ALBUM/ (no custom domain yet)
- Built with Hugo Extended + PaperMod theme
- Deployed via GitHub Actions on push to `main`

## Your Role Here

Content editor and Hugo technician. Tasks here are:
- Adding or editing gallery entries and posts
- Fixing Hugo/PaperMod configuration
- Managing the deploy workflow

## Hugo Conventions

- **Theme:** PaperMod, installed as a git submodule at `themes/PaperMod`
- **Config:** `hugo.toml` in root
- **Content:**
  - `content/posts/` — writeups, one folder per post
  - `content/gallery/` — image/portfolio entries
- **Page bundles:** prefer `content/<section>/<name>/index.md` with images local to that folder
- **Search page:** `content/search.md` — do not remove, PaperMod requires it
- **Build:** `hugo --minify` — always use Extended variant (required for PaperMod SCSS)

## Post Frontmatter

Every post/gallery entry must have:

```yaml
---
title: "Entry Title"
date: YYYY-MM-DD
description: "One sentence — used in listings and SEO."
tags: ["tag1", "tag2"]
author: "Dusan B. Jovanovic"
---
```

Optional cover image (local to entry folder):

```yaml
cover:
  image: "filename.jpg"
```

## Comments

Comments are currently **disabled** (`comments = false` in `hugo.toml`). DBJ_ICEBERG uses Giscus backed by GitHub Discussions — if comments are enabled here later, copy the `[params.giscus]` block and `layouts/_partials/comments.html` pattern from that repo, and enable Discussions on this repo first.

## Domain

No custom domain configured. `baseURL` points at the default GitHub Pages URL. If a custom domain is added later, add a `static/CNAME` file and update `baseURL` (see DBJ_ICEBERG for the pattern).

## Ownership

- &copy; dbj@dbj.org
- MIT License

## Behavioral Rules

1. **No padding.** No summaries, no affirmations.
2. **Do not invent URLs.**
