# Street Pulse Foundation — starter site

A no-framework static starter for `streetpulsefoundation.org` and the flagship `/blue/` program page.

## Why this version is intentionally static
This first release is designed to be simple for GitHub + Cloudflare Pages:
- no Node dependencies
- no framework install
- no build pipeline required
- easy for Muse or Codex to edit
- can later be migrated to Astro without changing the public URLs

## Pages
- `/` — Foundation home
- `/blue/` — StreetPulse Blue
- `/about/` — About
- `/partner/` — Partnership
- `/404.html`

## Cloudflare Pages settings
Use Git integration with the GitHub repository.

- Production branch: `main`
- Framework preset: None
- Build command: `exit 0` (Cloudflare recommends this for static sites when you do not need a build)
- Build output directory: `public`

The repository root contains the README and the deployable website lives inside `public/`.

## Custom domains
After the `*.pages.dev` deployment works:
1. Add `streetpulsefoundation.org` in Pages > Custom domains.
2. Because this is an apex domain, the domain must be a Cloudflare zone and the nameservers at Northwest must point to the two nameservers Cloudflare assigns.
3. Add `www.streetpulsefoundation.org` as a custom domain too.
4. Configure a Cloudflare Redirect Rule so `www.streetpulsefoundation.org/*` permanently redirects to `https://streetpulsefoundation.org/$1`.
5. Preserve all existing MX/TXT/DKIM/SPF/DMARC records when moving DNS.

## Before public promotion
Replace/verify:
- legal and tax status wording
- leadership / board information
- verified contact email
- donation processor URL
- real partner names only after authorization
- any impact statistics only after evidence exists
- social accounts
- photography / media
- privacy policy and transparency documents

## Editing
Shared styles are in `public/assets/styles.css`.
Shared mobile-menu logic is in `public/assets/site.js`.

## Important
Do not claim the Foundation is a 501(c)(3), that donations are tax-deductible, or that it has grants/partners/projects until those facts are verified.
