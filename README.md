# Redesigned site — drop-in files

Copy everything in this folder into the root of `yejinjkim.github.io`, replacing the
files of the same name. Then delete the old theme files you no longer need:
`_sass/`, `assets/css/style.scss`, `_includes/site-header.html`,
`_includes/social-metatags.html`, `_layouts/post.html`, `pages/lectures.md`,
`pages/funding.md` (their content now lives in the YAML data files).

Keep `assets/images/` and `assets/files/` exactly as they are.

## Where content lives now

| To edit | File |
| --- | --- |
| News items | `_data/news.yml` (newest first; homepage shows the first 5) |
| Team members | `_data/team.yml` |
| Research areas | `_data/research.yml` |
| Grants | `_data/funding.yml` |
| Courses | `_data/courses.yml` |
| CV blocks (career, honors, panels, service) | `_data/cv.yml` |
| Recruiting copy | `_data/opportunities.yml` |
| Bio prose | `index.md`, `pages/professor.md` |
| Nav | `_config.yml` (`header_pages`) |

Adding a news item is two lines in `_data/news.yml`; no HTML anywhere.

## Design

Colors, type and spacing come from `assets/css/modernist.css` (the Modernist token
sheet — do not hand-edit values in `site.css`; use `var(--color-*)` etc.).
