# DBJ Album

> A public album by Dusan B. Jovanovic — mixed media portfolio of work and writing.

**Live site:** https://dbjarh.github.io/DBJ_ALBUM/

## What this is

A portfolio of images and writeups.

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
