# ruchirchawdhry.github.io

Domain-root GitHub Pages site and discoverability infrastructure for public projects.

The [central sitemap workflow](https://github.com/RuchirChawdhry/ci-workflows/blob/main/docs/sitemap-index.md) discovers public GitHub Pages project sitemaps and deploys a root project directory, robots.txt, sitemap.xml (all discovered page URLs) and sitemaps.xml (index of individual sitemap files). It runs daily, on main pushes and on manual dispatch.

## Setup

- In Settings → Pages, set Source to GitHub Actions.
- Put Google Search Console HTML verification files in public/.
- Verify https://ruchirchawdhry.github.io/ as a URL-prefix property, then submit sitemaps.xml (or the consolidated sitemap.xml alone).

Project websites remain independently deployed; the root workflow does not modify them. The index includes only verified same-host XML sitemap files. Custom domains require separate sitemap submission.

[Root website](https://ruchirchawdhry.github.io/) · [All page URLs](https://ruchirchawdhry.github.io/sitemap.xml) · [Sitemap index](https://ruchirchawdhry.github.io/sitemaps.xml)

The central discovery job logs rejected sitemap sources to help diagnose missing project entries.

## Crawler policy

The generated [robots.txt](https://ruchirchawdhry.github.io/robots.txt) explicitly allows named AI, search, SEO and research crawlers, plus all other crawlers through a wildcard rule. It declares both root sitemaps and each discovered project sitemap. The policy is maintained in the central workflow.

## AI documentation index

[llms.txt](https://ruchirchawdhry.github.io/llms.txt) is a generated catalogue of project-level AI-readable documentation indexes. The central workflow discovers valid files automatically, includes repository descriptions, and refreshes the catalogue with the daily sitemap build. It does not require a manual project list.

## Reference documentation

- [Schema.org JSON-LD reference](docs/schema-org-reference.md) — selected schema types and agreed properties for automatic generation.
