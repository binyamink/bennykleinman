# bennykleinman.com

Personal academic website of Benny Kleinman, served with GitHub Pages.

## Structure

- `index.html` — the whole site (bio, contact, working papers, publications). Plain HTML, no build step.
- `photo.jpg` — profile photo (from Dropbox/CV/Benny Kleinman Portraits/headshot-4x5-1000.jpg).
- `stanford-wordmark.png` — official Stanford stacked wordmark (identity.stanford.edu), cardinal red.
- `cv.pdf` — CV (copy of Dropbox/CV/bk_CV.pdf); replace in place to update.
- `papers/` — paper PDFs hosted on the site (better for Google Scholar indexing than Drive/Dropbox links). Replace a file in place to update it; the address stays the same.
- `favicon.svg` — browser tab icon.
- `404.html` — "page not found" page; also forwards old file addresses (bk_JMP.pdf, bk_CV.pdf, …) that other sites still link to. Edit the REDIRECTS list in it to add more.
- `CNAME` — custom domain (www.bennykleinman.com).
- `.nojekyll` — tells GitHub Pages to serve files as-is.

## Updating

Each paper is one `<div class="paper">` block in `index.html`:

```html
<div class="paper">
  <a class="title" href="PAPER_URL">Paper Title</a>
  <span class="meta">with <a href="COAUTHOR_URL">Coauthor Name</a> · Revise and resubmit, <em>Journal Name</em></span>
  <span class="links">
    <a href="APPENDIX_URL">Online Appendix</a>
  </span>
</div>
```

To add a paper, copy a block and edit it. To move a paper from Working Papers to
Publications, cut the block and paste it into the `publications` section.
Commit to `main` and the site updates within about a minute.
