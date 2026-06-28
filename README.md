# Full Send Studios — public site (GitHub Pages)

Two static pages, safe to host publicly. **No costs, ROI, budgets, approvals, or file paths appear here** — those stay in the private Cowork console + Notion.

- `index.html` — **client-facing agency page** (the link you share with prospects).
- `ops/index.html` — **live ops mirror** (pipeline + board, throughput/quality only, no dollars).

## Before you publish — edit these
In `index.html`:
- Brand name `Full Send Studios` → your studio name (appears in the nav, footer, and `<title>`).
- The contact email — replace `CHANGE-ME@example.com`.
- The "In the studio now" line (hero) — current project + stage.

## Put it online (free) — ~5 minutes
1. Create a **GitHub account** if you don't have one (github.com). *(You do this — I can't create accounts or enter credentials.)*
2. Create a **new PUBLIC repo**, e.g. `gg-studio-site`. (Pages serves from public repos on the free plan.)
3. Upload the contents of this `site/` folder to the repo root (so `index.html` is at the top level and `ops/index.html` sits under it).
4. Repo **Settings → Pages → Build and deployment → Source: Deploy from a branch → `main` / root → Save.**
5. In ~1 minute your URLs are live:
   - Client page: `https://<your-username>.github.io/gg-studio-site/`
   - Live ops: `https://<your-username>.github.io/gg-studio-site/ops/`
6. *(Optional)* Custom domain: Settings → Pages → Custom domain (e.g. `studio.yourdomain.com`), then add the DNS record GitHub shows you.

## Keeping it current
This is a **static** site — it reflects the pipeline as of the last upload. When the studio state changes, I regenerate these two files and you re-upload (or, once a desktop git client / GitHub Desktop is set up, a one-click push). 

Want it to **auto-update live** instead? That needs a tiny serverless function (Netlify/Vercel free tier) that reads Notion server-side with a secret token and returns only the safe fields — so the token never touches the public page. Say the word and I'll prep that version.

## What stays PRIVATE (never put in this repo)
- The internal dashboard `sky-studio-production-control.html` (shows costs/ROI/budget/approvals).
- Notion IDs/tokens, agent souls, skills, client business data.
Keep those in your private Drive / Cowork only. If you also want version history of the agent souls + skills, put **those** in a **separate private repo** — not this public one.
