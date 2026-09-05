# tlmnhut.github.io

Personal academic site for Nhut Truong — <https://tlmnhut.github.io>

Jekyll, no theme gem. Typography is adapted from
[Tufte CSS](https://github.com/edwardtufte/tufte-css) via
[jekyll-theme-tufte](https://github.com/ab/jekyll-theme-tufte) (both MIT); ET Book (MIT) is
self-hosted under `assets/fonts/et-book/`, with its licence alongside it.

## Editing

| To change | Edit |
|---|---|
| Bio / intro text | `_pages/about.md` |
| News items | `_data/news.yml` |
| Research themes and their papers | `_projects/*.md` |
| Nav and profile links | `_data/navigation.yml` |
| Colours, fonts, column width | `_sass/_settings.scss` |

## Running the preview server

Start it (from the repo root):

```sh
JEKYLL_NO_BUNDLER_REQUIRE=1 jekyll serve --livereload
```

Then open <http://localhost:4000>. **Stop it with `Ctrl+C`** in that terminal.

`JEKYLL_NO_BUNDLER_REQUIRE=1` tells Jekyll to ignore the `Gemfile`, which pins
`github-pages` for parity with the live build but is not installed locally. To
drop the prefix, run `bundle install` once and then plain `jekyll serve` works.

### What reloads on its own, and what does not

While the server runs it watches the source and rebuilds on save. Edit, save,
refresh the browser — no restart needed for:

| Reloads automatically | Where |
|---|---|
| Bio / intro text | `_pages/about.md` |
| News items | `_data/news.yml` |
| Research themes and their papers | `_projects/*.md` |
| Nav and profile links | `_data/navigation.yml` |
| Colours, fonts, column widths | `_sass/*.scss` |
| Templates | `_layouts/`, `_includes/` |

**`_config.yml` is the exception.** Jekyll reads it once at startup and never
re-reads it, so a change there (site title, `author.bio`, `author.avatar`,
collections, plugins) shows nothing until you `Ctrl+C` and start the server
again. If an edit seems to have no effect, that is almost always why.

### If port 4000 is already taken

A server left running in another terminal still holds the port. Either find and
stop it:

```sh
ps -eo pid,args | grep "[j]ekyll serve"   # note the pid
kill <pid>
```

or just use a different port: `jekyll serve --port 4001`.

Avoid `pkill -f "jekyll serve"` — the pattern matches the shell running it too,
so it can kill your own terminal.

## Deploying

GitHub Pages builds `master` automatically; there is no workflow file. Push when
the local preview looks right.
