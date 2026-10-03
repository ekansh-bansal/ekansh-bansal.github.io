# ekansh-bansal.github.io

Personal site, built as a set of interchangeable **views** (themes).

## Layout

```
index.html                  ← the current default view (a copy of its theme file)
themes/
  index.html                ← the "Views" page listing every theme
  themes.json               ← theme registry (id, name, path, default)
  sky-islands/index.html    ← Sky Islands view — floating islands, one day across the scroll
assets/                     ← logos shared by every view
parkly-*.html               ← Parkly case studies, linked from the views
LICENSE-OFL.txt             ← font licences for the case-study pages
```

## Adding a new view

1. Create `themes/<id>/index.html`. Use root-absolute paths (`/assets/…`, `/parkly-…html`, `/favicon.svg`) so the same file works from any folder.
2. Add an entry to `themes/themes.json` and a card to `themes/index.html`.
3. To make it the homepage, copy it over `/index.html` and update `"default"` in `themes.json`.
