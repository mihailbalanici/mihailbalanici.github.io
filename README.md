# Mihail Balanici — personal site

A Jekyll site for GitHub Pages. No build setup is needed: push it to your
`username.github.io` repository and GitHub builds it automatically.

## Put it online

1. Upload the contents of this folder (not the folder itself) to the root of your
   `username.github.io` repository.
2. In the repo go to **Settings → Pages** and set the source to **Deploy from a branch → main → / (root)**.
3. Your site appears at `https://username.github.io` after a minute or two.
4. For your own domain, follow the custom-domain steps (Settings → Pages → Custom domain),
   and set `url:` in `_config.yml` to `https://firstnamelastname.com`.

## Things to fill in

| What | Where |
|---|---|
| GitHub, ResearchGate and ORCID links (marked `TODO`) | `_config.yml` → `social:` |
| Your own "About me" text | `index.html` (the `about` section) |
| Your domain | `_config.yml` → `url:` |

Leave a social link empty (`""`) to hide its icon.

## Where each section's content lives

Most content is in simple YAML files, so you rarely touch HTML:

| Page | Edit |
|---|---|
| About (experience, education) | `_data/experience.yml`, `_data/education.yml`, `index.html` |
| Publications | `_data/publications.yml` |
| Skills | `_data/skills.yml` |
| Certifications & awards | `_data/certifications.yml` |
| Projects | `_data/projects.yml` |
| Blog | add Markdown files to `_posts/` named `YYYY-MM-DD-title.md` (see the sample post) |
| Photography | drop `.jpg` / `.png` / `.webp` files into `assets/photos/` — they appear automatically. Resize to ~2000 px on the long side first so pages load quickly. |
| CV download | replace `assets/cv/Mihail_Balanici_CV.pdf` |
| Profile photo | replace `assets/img/profile.jpg` (square image) |

## Preview locally (optional)

With Ruby installed:

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.
