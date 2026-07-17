# driveycar-site

Deploy repo for **driveycar.com** (GitHub Pages under the `zenfosec` account).

**The source of truth is `driveycar/site/`** — edit the pages there and copy them here to publish.
This folder holds only the public pages that get served. Right now that is the **Phase 1 vague
placeholder set** (pre-App-Store-approval — deliberately says nothing about what the game is):

- `index.html` — teaser page → `https://driveycar.com`
- `support.html` — support + FAQ → `https://driveycar.com/support.html` (App Store **Support URL**)
- `privacy.html` — privacy policy → `https://driveycar.com/privacy.html` (App Store **Privacy Policy URL**)
- `terms.html` — terms of service → `https://driveycar.com/terms.html`

Self-contained static pages: inline CSS, **no external requests**, no build step.

**Do not copy anything from `driveycar/site/marketing/` here before Apple approves the app.** The
post-approval swap (Phase 2) is a single documented copy step — see Step F in
`driveycar/site/DEPLOY.md`.

## Status
Staged, files only — **no `git init`, no remote, and no `CNAME` file yet.** The full publish
walkthrough (init → `gh repo create driveycar-site --push` → enable Pages → deploy without CNAME first
for the `zenfosec.github.io/driveycar-site/` fallback → Namecheap DNS → add `CNAME` → Enforce HTTPS →
verify) lives in `driveycar/site/DEPLOY.md`. The `CNAME` file is added in that walkthrough's Step C,
*after* DNS — not now.
