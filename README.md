# Neural Chronicals

Neural Chronicals is a monthly digital magazine focused on AI, agentic AI, and AI systems.

This repository is the root project workspace for:
- The live publication site in `app/`
- Multi-agent handoff and run artifacts
- Issue research packages and media assets
- Cloudflare deployment configuration

## Repository Structure

- `app/` - Main publication web app (React + Vite + TypeScript)
- `app_2/` - Template copy for future publication experiments
- `issue_2/` - Issue 02 research package, Kimi artifacts, and data tables
- `security/` - Security notes and workflow snippets
- `handoff.md` - Cross-agent coordination log (append-only)
- `wrangler.toml` - Cloudflare Workers deployment config

## Root Scripts

From repository root:

- `npm run build` - Installs app dependencies and builds `app/dist`
- `npm run lint` - Runs lint checks for `app/`
- `npm run deploy` - Builds and deploys with Wrangler

## App Development

To work directly on the publication app:

1. `cd app`
2. `npm run dev`

Default local dev URL is usually `http://localhost:5173`.

## Deployment

Production deployment is configured at the repository root and uses Cloudflare Workers with static assets from `app/dist`.

- Build output: `app/dist`
- Deploy config: `wrangler.toml`
- Deploy command: `npm run deploy`

## Notes

- `.kindred/` stores local orchestration/runtime artifacts. See `.kindred/README.md`.
- Runtime `.kindred` paths are ignored by git.
- If sanitized fixtures are needed for docs/tests, commit only approved fixture artifacts.
