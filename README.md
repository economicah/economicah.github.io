# micahvillarreal.com

Source for [micahvillarreal.com](https://micahvillarreal.com), built with Jekyll on GitHub Pages. Every push to `main` republishes the site automatically within a few minutes.

## Where to edit

| What | File |
| --- | --- |
| About paragraph, contact links | `_includes/sections/about.md` |
| Papers, works in progress, pre-doctoral work | `_includes/sections/research.md` |
| Teaching and student feedback | `_includes/sections/teaching.md` |
| Talks by year | `_includes/sections/talks.md` |
| Hero (name, title, affiliation, icon links) and section order | `_layouts/default.html` |
| Site title and description (search previews) | `_config.yml` |
| Colors, fonts, spacing | `assets/css/main.css` |

The section files are plain Markdown. Edit them on GitHub, commit, and the site rebuilds. The "Last updated" date in the footer is set automatically at build time.

## Updating the CV or job market paper

Upload the new file under the **same filename** so existing links keep working:

- CV: `Villarreal, Micah.pdf`
- Job market paper: `MV_jmp_2025_latest.pdf`

To use a different filename, also update the links in `_layouts/default.html` (CV) or `_includes/sections/research.md` (paper).

## Adding a paper

Copy one of the `<article class="paper">` blocks in `_includes/sections/research.md` and change the title, link and abstract. Remove the `<span class="paper-tag">` line unless the paper needs a label.

## Headshot

The site uses `assets/img/headshot.jpg` (600 px wide). Replace it with another JPEG of about the same size and a 2:3 aspect ratio.

## Previewing locally (optional)

```
gem install jekyll jekyll-seo-tag kramdown-parser-gfm webrick
jekyll serve
```

Then open <http://localhost:4000>.
