# Yukai Tang's academic website

A small Jekyll website with a banner and horizontal navigation inspired by
[Jingyi Zhuo's website](https://jingyizhuo.github.io/).

## Customize

- Edit `_config.yml` for your name, optional role and affiliation, description,
  banner, and contact links. The banner reuses an Unsplash landscape image from
  the previous theme. Add your own image to `site/assets/images/` and update
  `banner_image` to replace it.
  Empty optional links are hidden. `email` is an email address; the other social links
  are full URLs. Set `cv_pdf` to a local PDF path or a full URL when your CV is ready.
- Edit the Markdown pages in `site/_pages/` to add your biography, research,
  publications, resources, and CV. Replace bracketed placeholders with your details.
- Edit `site/_data/navigation.yml` to change the horizontal navigation.
- Put images and PDFs in `site/assets/`, then link to them with paths such as
  `/assets/images/photo.jpg` or `/assets/pdf/cv.pdf`.

The previous al-folio files are retained outside `site/` for reference. Jekyll uses
`source: site`, so those demo pages, assets, and plugins are not published.
The archived al-folio instructions in `CUSTOMIZE.md` and `INSTALL.md` do not apply
to this new template.

## Local preview

Install Ruby 3.3 or newer and Bundler, then run from the repository root:

```sh
bundle install
bundle exec jekyll serve --livereload
```

Open <http://localhost:4000>. Restart the server after changing `_config.yml`.
To check the production build:

```sh
JEKYLL_ENV=production bundle exec jekyll build
```

The generated website is written to `_site/`.

## Deployment

Push changes to `main` or `master`. The Deploy site workflow builds the website
and publishes `_site/` to the `gh-pages` branch. Pull requests build for validation
without publishing. You can also run the workflow manually from GitHub Actions.

In the repository's **Settings → Pages**, select **Deploy from a branch**, then
choose **gh-pages** and **/ (root)**. The site address is
<https://Negotch.github.io/>; keep `baseurl` empty for this user website.
