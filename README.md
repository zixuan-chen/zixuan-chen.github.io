# zixuan-chen.github.io

Personal academic homepage of **Zixuan Chen** — built with
[Jekyll](https://jekyllrb.com/) on top of the
[Academic Pages](https://academicpages.github.io/) theme (a fork of
[Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)).

Live site: <https://zixuan-chen.github.io>

---

## Repository layout

| Path | What it controls |
| --- | --- |
| `_config.yml` | Site-wide settings: title, description, social preview, author info and sidebar links |
| `_pages/about.md` | The homepage content (bio, research interests, news, publications, education, services) |
| `_data/navigation.yml` | Header navigation links |
| `_sass/_custom.scss` | Site-specific styles for the homepage (news list, publication list, link buttons) |
| `assets/css/main.scss` | Imports every `_sass` partial, including `_custom.scss` |
| `_includes/` | Theme partials, e.g. `seo.html` (meta tags) and `footer/custom.html` |
| `images/` | Avatar, favicons, and `og-image.png` (1200x630 social preview) |
| `files/` | Static downloads such as the CV PDF |

## Editing content

### Add a publication

Copy an existing `<div class="pub-item">` block in `_pages/about.md` and edit
the title, authors, venue, and link buttons. Conventions used on this page:

- `*` marks equal contribution, `#` marks the corresponding author
- `M<sup>3</sup>-VOS` renders as M³-VOS
- Button classes are `btn-box`; any `<a href="...">` with that class renders as
  a pill button

### Add a news item

Append a `<li>` inside `.news-container` in `_pages/about.md`:

```html
<li>
  <span class="news-date">2026.01</span>
  <span><span aria-hidden="true">🎉</span><span class="sr-only">Announcement:</span> "Paper" was accepted to&nbsp;<strong>Venue</strong>.</span>
</li>
```

Newest entries go first. The list is scrollable, so it stays compact.

### Add the CV

Upload your PDF to `files/Zixuan_Chen_CV.pdf`. The **CV** item in
`_data/navigation.yml` already points at that exact path.

### Sidebar links

Add handles under `author:` in `_config.yml` (`twitter`, `linkedin`, `orcid`,
`semantic`, …). Icons render automatically for the keys supported by
`_includes/author-profile.html`.

## Local preview

Requires Ruby 3.x, Bundler, and Node.js:

```bash
bundle install
bundle exec jekyll serve -l -H localhost
# http://localhost:4000
```

Changes to Markdown and HTML reload automatically; changes to `_config.yml`,
`_sass/`, or `_includes/` require restarting the server.

## Deployment

Pushing to `master` triggers the built-in GitHub Pages build ("pages build and
deployment" workflow) and the site goes live at
<https://zixuan-chen.github.io> within a minute or two. No manual build step is
needed.

## Notes

- The theme's own README, issue templates, and sample content were removed —
  this repository only contains this site's content and configuration.
- `_sass/_custom.scss` is imported last in `assets/css/main.scss` so its rules
  override the theme defaults.
- Social preview (`og:image`) comes from `images/og-image.png` via the
  `og_image` key in `_config.yml`.

## License and credits

Theme © [Stuart Geiger](https://github.com/staeiou), based on Minimal Mistakes
by [Michael Rose](https://mademistakes.com/), MIT licensed — see `LICENSE`.
Content and images © Zixuan Chen.
