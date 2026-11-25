# ruchirchawdhry.github.io

Domain-root GitHub Pages site and discoverability infrastructure for public projects.

The [central sitemap workflow](https://github.com/RuchirChawdhry/ci-workflows/blob/main/docs/sitemap-index.md) discovers public GitHub Pages project sitemaps and deploys a root project directory, robots.txt, sitemap.xml and sitemap-root.xml. It runs daily, on main pushes and on manual dispatch.

## Setup

- In Settings → Pages, set Source to GitHub Actions.
- Put Google Search Console HTML verification files in public/.
- Verify https://ruchirchawdhry.github.io/ as a URL-prefix property, then submit sitemap.xml.

Project websites remain independently deployed; the root workflow does not modify them. The index includes only verified same-host XML sitemap files. Custom domains require separate sitemap submission.

[Root website](https://ruchirchawdhry.github.io/) · [Sitemap](https://ruchirchawdhry.github.io/sitemap.xml)
