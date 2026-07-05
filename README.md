# jeevanto-ops-console

Static hosting for the Jeevanto internal ops console, served at
**https://ops.jeevanto.com** via GitHub Pages.

This repo contains **one static file** (`index.html`) that holds **no secrets** —
it talks to the `ops-dashboard` Supabase edge function, which is the only place the
`service_role` key lives. The browser holds only a post-login session token.

Source of truth: `tools/ops-dashboard/index.html` in the private Jeevanto repo
(Phase 33.4). This repo is a publish target; do not edit here by hand.
