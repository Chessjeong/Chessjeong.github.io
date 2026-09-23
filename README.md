# Minho Jeong

Personal academic website built with Jekyll.

**[chessjeong.github.io](https://chessjeong.github.io/)**

## Local development

Requires Ruby 3.3 and Bundler.

```sh
bundle install
bundle exec jekyll serve --livereload
```

Open [localhost:4000](http://localhost:4000). Restart the server after changing `_config.yml`.

## Editing content

| Content | Location |
| --- | --- |
| Biography, contact details, education, and experience | `_data/profile.yml` |
| Publications | `_publications/` |
| Projects | `_data/projects.yml` |
| Background section order and layout | `_data/background_sections.yml` |
| Navigation | `_data/navigation.yml` |
| Homepage layout | `index.html` |
| Styles | `assets/css/custom.css` |
| CV | `assets/files/minho-jeong-cv.pdf` |

Set `selected: true` in a publication's front matter to feature it on the homepage.

## Deployment

Pushes to `main` build and deploy the site to GitHub Pages. Pull requests run the build without deploying.

To check the build locally:

```sh
bundle exec jekyll build
```

Based on [luost26/academic-homepage](https://github.com/luost26/academic-homepage). See [LICENSE](LICENSE).
