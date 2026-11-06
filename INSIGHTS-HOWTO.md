# Publishing an Insight

Insights are written as simple text files (Markdown). GitHub Pages turns them into
styled article pages automatically when you push. No HTML needed.

## To publish a new article

1. Copy `_drafts/example-insight.md` into the `_posts/` folder.
2. Rename it: `YYYY-MM-DD-short-title.md` (e.g. `2026-11-20-hst-on-new-rentals.md`).
   - The date is the publication date shown on the article.
   - The short title becomes the web address: `northernadvisory.ca/insights/hst-on-new-rentals/`.
3. Edit the top block (between the `---` lines):
   - `title:` the article headline
   - `description:` one or two sentence summary (used on cards and in search/LinkedIn previews)
   - `category:` a short label, e.g. Tax, Real Estate, Reporting, Advisory
   - `image:` optional banner photo; put the file in `assets/insights/`
4. Write the article underneath. See the draft template for headings, lists, links, and tables.
5. Commit and push. The article appears on `/insights/` (newest first) within a minute or two.

## Good to know

- Files in `_drafts/` are never published. Keep work-in-progress there.
- A post dated in the future will not appear until that date (after the next push).
- Each article automatically gets: reading time, author box, legal disclaimer,
  "More insights" links, sitemap entry, and an RSS feed entry (`/insights/feed.xml`).
- To change the disclaimer or author box, edit `_layouts/insight.html`.
- `linkedin:` (optional) adds a "first shared on LinkedIn" link under the article.
- `share_image:` (optional) sets the preview picture used when the article is shared.
- Financial statement tables: copy a `<figure class="statement">` block from
  `_posts/2026-09-21-indirect-cash-flow-statement.md`. Row classes: `head` (bold label),
  `sub` (italic sub-heading), `hl` (gold highlight), `subtotal`, `total` (double underline);
  label indent levels `l1` to `l4`. Tables built this way stay sharp and fit on phones.
- Avoid em dashes (—) in copy. Typing `--` or `---` in Markdown also turns into dashes.
