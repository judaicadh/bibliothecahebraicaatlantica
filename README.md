# Bibliotheca Hebraica Atlantica
Tracking Libraries that Contain Books with Hebrew in the Atlantic World

## About the Project (completed May 2017)
The presence of Latin and Greek texts as well as Hebrew Bibles in colonial American libraries is well documented. What lacks systematic documentation are other kinds of Oriental, Hebraic and rabbinic texts that shared the shelves with them. This project aims to explore volumes of such texts that crossed the Atlantic during the seventeenth and eighteenth centuries and were available as reading materials in institutional and private libraries. Though hidden in plain sight, recognition of these libraries of “Christian rabbinism” - that is, Christian interest in post-Biblical Jewish history and in comparative Semitic scholarship, and its arrival in the Western Hemisphere - requires a shift of attention that now has become possible thanks to a new generation of research on the subject. Christian learning about Judaism as a chapter in the early modern history of scholarship, however, has mainly focused on the European context. How and when this prodigious output, this first wave of scholarly migration, crossed the Atlantic and took root in the colonial Americas still remains to be framed.

### Partners
- Laura Newman Eckstein
- John Pollack
- Peter Stallybrass (Penn)
- Michelle Margolis, Columbia University Libraries
- James Green and the staff of the Library Company of Pennsylvania
- the staff of the Historical Society of Pennsylvania
- Jesús de Prado Plumed, Universidad Nacional Autónoma de México
- Oliver Mitchell-Boyask

---

## The website

The project is published as a static [Jekyll](https://jekyllrb.com/) site, built and hosted on
**[Netlify](https://www.netlify.com/)** at
**https://bibliothecahebraicaatlantica.judaicadhpenn.org**. Each library's holdings are stored as CSV
data and rendered as searchable, sortable, mobile-friendly tables using
[DataTables](https://datatables.net/).

### Repository structure

| Path | What it holds |
|------|---------------|
| `index.html` | Home page (project overview). |
| `_docs/` | One Markdown page per library/collection (Franklin, Yale, Jefferson, …). Front matter + the table markup. |
| `_data/` | The underlying data, one `*.csv` per library, referenced by the matching page via `site.data.<Name>`. |
| `_layouts/` | Page templates. `docs.html` renders the data-table pages. |
| `_includes/` | Reusable partials: `head.html`, `topnav.html`, `footer.html`, `analytics.html`, nav includes. |
| `_sass/`, `css/` | Bootstrap 3 + the Bootswatch "Journal" theme, compiled to `css/main.css`. |
| `_config.yml` | Site-wide settings (title, base URL, plugins, analytics ID). |

### Adding or updating a library

1. Add the data as `_data/<Library_Name>.csv` (column headers become the table columns).
2. Create `_docs/<Library Name>.md`. The quickest path is to copy an existing page (e.g.
   `_docs/Benjamin Franklin.md`) and update its front matter:
   ```yaml
   ---
   title: Library Name
   permalink: /docs/librarypermalink/
   csvlink: https://github.com/judaicadh/bibliothecahebraicaatlantica/blob/master/_data/Library_Name.csv
   textlink: "Full bibliographic citation of the source catalogue."
   textview: https://link-to-the-source
   ---
   ```
   Then point the table loop at your data: `{% for entry in site.data.Library_Name %}`.
3. Commit and push to `master` — Netlify rebuilds and deploys automatically (usually within a minute).

Small text edits can be made directly in the GitHub web editor; structural changes are easier to
preview locally first (see below).

### Running the site locally

Requires **Ruby 3.x** (the toolchain no longer builds on macOS's system Ruby 2.6 — use
[rbenv](https://github.com/rbenv/rbenv) or similar).

```bash
bundle install
export LANG=en_US.UTF-8          # avoids a Sass "US-ASCII character" build error
bundle exec jekyll serve
# → http://localhost:4000/
```

### Deployment

The live site is built and hosted on **[Netlify](https://www.netlify.com/)** (config in
[`netlify.toml`](netlify.toml)): every push to `master` runs `bundle exec jekyll build` and publishes
`_site`. The Ruby version is pinned in [`.ruby-version`](.ruby-version). Jekyll and its plugins are
pinned via the [`github-pages`](https://github.com/github/pages-gem) gem — refresh occasionally with
`bundle update github-pages`.

### Analytics

Page traffic is tracked with **Google Analytics 4**. Set your Measurement ID in `_config.yml`:

```yaml
google_analytics: G-XXXXXXXXXX
```

The snippet (`_includes/analytics.html`) only loads on the live production build, so local development
traffic is never counted. Leave the value blank to disable tracking entirely.

---

# This is a Judaica Digital Humanities at the Penn Libraries repository.
Judaica Digital Humanities at the <a href="http://library.upenn.edu">Penn Libraries</a> (also referred to as Judaica DH) is a robust program of projects and tools for experimental digital scholarship with Judaica collections, informed by digital humanities, Jewish studies, and cultural heritage approaches. Visit our [website](judaicadh.github.io).
