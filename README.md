# bennykleinman.com

Personal academic website of Benny Kleinman, served with GitHub Pages.

## Structure

- `index.html` — the whole site (bio, contact, working papers, publications). Plain HTML, no build step.
- `photo.jpg` — profile photo.
- `.nojekyll` — tells GitHub Pages to serve files as-is.

## Updating

Each paper is one `<p class="paper">` block in `index.html`:

```html
<p class="paper">
  <a class="title" href="PAPER_URL">Paper Title</a>, with
  <a class="coauthor" href="COAUTHOR_URL">Coauthor Name</a>
  <span class="extra">
    <a href="APPENDIX_URL">[Online Appendix]</a>
  </span>
  <span class="venue">Revise and resubmit, <em>Journal Name</em></span>
</p>
```

To add a paper, copy a block and edit it. To move a paper from Working Papers to
Publications, cut the block and paste it under the `PUBLICATIONS` comment.
Commit to `main` and the site updates within about a minute.
