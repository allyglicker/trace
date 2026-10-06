# Trace — Base44 dev environment

## What this is
A single-file static web app (`index.html`). No backend, no build step, no
package manager, no external services or credentials. Everything runs in the
browser (camera + canvas edge detection).

## Running it
`docker compose -f docker-compose.base44.yml up -d` — serves `index.html` via
nginx on host port 3000. The repo is bind-mounted read-only, so edits to
`index.html` are visible on browser refresh (no rebuild needed).

## Notes
- The camera requires HTTPS; the preview proxy provides that automatically.
- No tests, no migrations, no seeds.
