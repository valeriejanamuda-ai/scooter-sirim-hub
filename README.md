# Scooter SIRIM Compliance Hub

A shareable, browser-viewable hub for all Malaysia e-scooter / SIRIM import &
approval guides and official reference documents. One link — click a topic —
the guide or PDF opens directly in the browser. No need to open local files.

## Public link

> https://it-awesomeree.github.io/scooter-sirim-hub/

Share this single URL with the team.

## What's inside

| Folder | Contents |
|---|---|
| `index.html` | The hub landing page (start here) |
| `latest/` | 8 current guides — dated 19 May 2026 (recommended) |
| `archive/` | 7 earlier v1 guides — dated 18 May 2026 (superseded, kept for record) |
| `docs/` | 10 official reference PDFs (SIRIM, MITI, KPDN, ePermit) |
| `style.css` | Site styling (pure CSS, no JavaScript) |

The **Master Scenario Matrix** (`latest/master-scenario-matrix.html`) is the
"start here" decision table.

## One-time setup (after first push)

In the GitHub repo: **Settings → Pages → Build and deployment → Source =
"GitHub Actions"**. After that, every push to `main` auto-deploys via
`.github/workflows/pages.yml` (no build step — static files served as-is).

## Updating a guide later

1. Replace / add the file in `latest/`, `archive/` or `docs/` (keep
   kebab-case filenames — no spaces).
2. If it's a new topic, add a matching card in `index.html`.
3. Update the `Last updated` date in `index.html`.
4. `git add -A && git commit -m "update guides" && git push` — the site
   redeploys automatically within a minute.

## Source

Synced from the local `Scooter SIRIM` reference set:
latest = 19 May 2026, archive = 18 May 2026.
