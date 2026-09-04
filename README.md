# tlmnhut.github.io

Personal academic site for Nhut Truong — <https://tlmnhut.github.io>

Jekyll, no theme gem. Typography is adapted from
[Tufte CSS](https://github.com/edwardtufte/tufte-css) via
[jekyll-theme-tufte](https://github.com/ab/jekyll-theme-tufte) (both MIT); ET Book (MIT) and
Lato (SIL OFL) are self-hosted under `assets/fonts/`, with their licences alongside them.

## Editing

| To change | Edit |
|---|---|
| Bio / intro text | `_pages/about.md` |
| News items | `_data/news.yml` |
| Research themes and their papers | `_projects/*.md` |
| Nav and profile links | `_data/navigation.yml` |
| Colours, fonts, column width | `_sass/_settings.scss` |

## Local preview

With the system Jekyll (3.8.6 here) and no bundle installed:

```sh
JEKYLL_NO_BUNDLER_REQUIRE=1 jekyll serve --livereload   # http://localhost:4000
```

The env var tells Jekyll to ignore the `Gemfile`, which pins `github-pages` for parity with the
live build. To drop it, install that bundle once (`bundle install`) and plain `jekyll serve` works.
Local builds also need `jekyll-redirect-from` (`gem install --user-install jekyll-redirect-from`).

GitHub Pages builds `master` automatically; no workflow file is needed.
