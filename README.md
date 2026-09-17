# Kivo website

The public Kivo website and Mac download.

Visit **https://kivo.com.ai/**.

The public landing page uses Cloudflare DNS and the GitHub Pages custom domain
`kivo.com.ai`. Its assets are built at the domain root; keep `docs/CNAME` in
every deployment. The previous GitHub Pages address redirects to this domain.
The account and API service stay on their own HTTPS hosts (for example
`account.kivo.com.ai` and `api.kivo.com.ai`); GitHub Pages only serves the
static landing page and download.

GitHub Pages publishes the `docs/` folder on `main`. The site supports English and German and follows the visitor’s system language.

This repository contains only the generated website and downloadable Mac app. The application source is maintained separately.

The Kivo 0.26.3 (build 52) Mac download is a Developer ID signed, Apple-notarized DMG. Open it and drag Kivo into Applications. It requires macOS 26 or later on Apple silicon.

Version 0.26.3 applies the same compiler-cache filtering when accepting a result and when saving its timeline snapshot, including project-prefixed cache folders. Source files, data and finished app bundles remain included; file and size limits still apply. You can retry saving a result locally without restarting the agent. Account sign-in and beta access run on the separate account/API services; this repository contains no account data or secrets.
