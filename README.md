# alfaj10408.github.io

Source for [alfaj10408.github.io](https://alfaj10408.github.io/), the academic website of Alfaj Uddin Ahmed
(Ph.D. student, Weldon School of Biomedical Engineering, Purdue University).

Built with [Hugo](https://gohugo.io/) and the open-source
[HugoBlox Academic CV template](https://github.com/HugoBlox/hugo-theme-academic-cv) (MIT License, © Lore Labs;
see [LICENSE.md](LICENSE.md)). Deployed to GitHub Pages by the workflow in `.github/workflows/deploy.yml` on
every push to `main`.

## Where things live

| What | File(s) |
| --- | --- |
| Name, bio, links, education, experience, skills, awards | `data/authors/me.yaml` |
| Homepage sections (research areas, publication list, projects, contact) | `content/_index.md` |
| Publications (one folder per paper) | `content/publications/<slug>/index.md` |
| Projects (one folder per project) | `content/projects/<slug>/index.md` |
| Experience page layout | `content/experience.md` |
| Downloadable CV | `static/uploads/alfaj-uddin-ahmed-cv.pdf` |
| Headshot and favicon | `assets/media/authors/me.png`, `assets/media/icon.png` |
| Site settings (title, theme, header, footer) | `config/_default/params.yaml`, `hugo.yaml`, `menus.yaml` |

## Updating

- **New publication:** copy an existing folder under `content/publications/`, edit `title`, `authors`, `date`,
  `publication_types` (`manuscript` while under review or in preparation; `paper-conference` or
  `article-journal` once published), `publication.name`, `abstract`, and `links`. Add `cite.bib` and a PDF
  to the same folder to get automatic Cite and PDF buttons.
- **Paper status changes:** edit `publication.name` (e.g. "Under review at ICLR 2027" → "ICLR 2027") and
  `publication_types`, and update the matching line in `data/authors/me.yaml` and `content/_index.md`.
- **New project:** copy a folder under `content/projects/`, edit the front matter and summary.
- **New CV:** replace `static/uploads/alfaj-uddin-ahmed-cv.pdf` (keep the filename, it is linked from the menu).

## Local preview

Requires Hugo Extended 0.162.0, Go, and Node 22 (Hugo fetches HugoBlox modules through Go).

```bash
npm install            # Tailwind CLI and Pagefind
hugo server            # http://localhost:1313
hugo --minify          # production build into public/
```
