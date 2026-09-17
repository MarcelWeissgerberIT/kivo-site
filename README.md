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

The Kivo 0.26.1 (build 50) Mac download is a Developer ID signed, Apple-notarized DMG. Open it and drag Kivo into Applications. It requires macOS 26 or later on Apple silicon.

Version 0.26.1 adds explicit continuation of failed or stopped tasks, persistent failure explanations, early agent-session recovery and reliable handling of larger Codex responses. Task files, usage and permission budgets stay with the existing task. Account sign-in and beta access run on the separate account/API services; this repository contains no account data or secrets.
