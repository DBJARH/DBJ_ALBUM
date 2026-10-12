# DBJ Album

**Live site:** https://media.dbj.org/

## What this is

> A public album by Dusan B. Jovanovic — mixed media portfolio

## Structure

- Home page content comes from `content/_index.md` (title + description only,no body). 
- The **home page layout** is in: `layouts/index.html`
  - It renders that content and then a grid of cards linking to each themed gallery section under  `content/gallery/` (e.g. ai-agents`, `tech-debt-legacy`, `ea-bpt`, `misc`).
- Each gallery section is a page bundle (`content/gallery/<theme>/index.md`
  with images stored alongside it) rendered via the `{{< gallery >}}`
  shortcode.

## Built with

- [Hugo](https://gohugo.io/) + [PaperMod](https://github.com/adityatelange/hugo-PaperMod)
- Deployed via GitHub Actions to GitHub Pages

---

&copy; dbj@dbj.org | MIT License | CC BY SA 4.0
