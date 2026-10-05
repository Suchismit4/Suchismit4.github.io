# Agent guidelines for Suchismit Ghosh's site

This is Suchismit4/Suchismit4.github.io, a personal GitHub Pages site using the official al-folio v1 starter. The public domain is suchismit.me and baseurl is empty. Never create a pull request against Academic Pages or upstream al-folio for personal site changes.

Keep content in \_pages, \_projects, \_news, and \_data. Runtime layouts, styling, and assets come from pinned al-folio gems in Gemfile; use configuration before adding local overrides. Keep Gemfile plugin dependencies and \_config.yml activation in agreement.

Use bundle exec jekyll build and npm run lint:style-contract to validate. Deployment builds the source on master/main and publishes generated output to gh-pages. Never hand-edit \_site or gh-pages. Preserve CNAME and personal assets. Do not invent credentials, dates, publications, or contact information.

See docs/INSTALL.md and docs/BOUNDARIES.md for upstream guidance; the upstream demo baseurl /al-folio does not apply to this user site.
