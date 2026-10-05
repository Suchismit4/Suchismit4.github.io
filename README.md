# Suchismit Ghosh

Personal academic website for [Suchismit Ghosh](https://suchismit.me), based on the official [al-folio](https://github.com/alshedivat/al-folio) v1 starter at commit `40c06007dab344970b681ba63b2241b1a8209ec1`. Runtime gems are pinned in `Gemfile` and `Gemfile.lock`.

The source repository remains `Suchismit4/Suchismit4.github.io`. `url` is the public custom domain, `baseurl` is empty, and `CNAME` is copied to the deployed site. The deployment workflow publishes to `gh-pages`; GitHub Pages must serve that branch's root.

Content: `_pages/about.md`, `_pages/work.md`, `_pages/writing.md`, `_projects/`, `_news/`, and `_data/cv.yml`. Replace `assets/img/profile.png` with your portrait when ready; the preserved existing file is a placeholder image. No personal email address or resume PDF existed in the old site, so the resume is rendered from confirmed CV data. News dates use year-only presentation because only years were supplied.

For local development, use `docker compose up --build`, or with Ruby 3.3+ and Bundler installed, run `bundle install` and `bundle exec jekyll serve`. Local overrides are limited to `_includes/news.liquid` for year-only dates and `assets/css/main.scss` for restrained typography, muted colors, smaller social links, and subtle portrait styling. The main stylesheet retains upstream Sass imports. Reviewed hashes are tracked in `.al-folio-overrides.yml`. The CI production build uses `bundle exec jekyll build`, followed by the upstream PurgeCSS step. See [upstream installation documentation](docs/INSTALL.md).

The Academic Pages files were inspected before replacement. Its PDFs, publications, CV, posts, and other example assets were boilerplate; the existing profile image was preserved byte-for-byte.
