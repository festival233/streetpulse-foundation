# StreetPulse Foundation — Website


Official website of the **StreetPulse Foundation** ("Street Pulse Foundation Inc.", a Delaware nonprofit corporation), served at [streetpulsefoundation.org](https://streetpulsefoundation.org).


## Architecture


- **Source of truth:** this GitHub repository (`main` branch)
- **Hosting:** Cloudflare Pages (auto-deploys on every push to `main`)
- **DNS:** Cloudflare
- **Domain registration:** Northwest Registered Agent


## Site


Pure static HTML/CSS/JS — no build step. Cloudflare Pages settings:


| Setting | Value |
|---|---|
| Framework preset | None |
| Build command | *(empty)* |
| Build output directory | `/` |
| Root directory | `/` |
| Production branch | `main` |


## Making changes


Edit any file in this repo and push to `main` — Cloudflare Pages rebuilds and publishes automatically within a minute or two.


## Structure


```
index.html        Homepage
about.html        About the Foundation
programs.html     Program areas
contact.html      Contact information
404.html          Not-found page
css/styles.css    All styles
js/main.js        Mobile nav toggle
robots.txt        Crawler rules
sitemap.xml       Sitemap
_headers          Cloudflare Pages security headers
```


## Notes


- Only verified organizational facts belong on this site. Do not claim 501(c)(3) status until the IRS determination letter is received; the site states "Federal 501(c)(3) tax-exempt recognition in progress."
- The Foundation maintains complete legal, financial, and operational separation from any for-profit entities.

Pipeline verified: 2026-10-02.
