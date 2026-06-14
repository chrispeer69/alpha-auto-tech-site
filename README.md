# Alpha Auto Tech — Marketing Site

Single-page marketing site for **Alpha Auto Tech** by Blue Collar AI. One native platform that replaces three legacy auto-shop systems (Mitchell 1, BOLT ON Technology, SideKick360) — matched feature-for-feature, then beaten, with an AI layer none of them have.

## What's here

- `index.html` — the full site (matchups, deck slider, video, audio, CTAs)
- `slides/` — 12 deck slides powering the auto-advancing walkthrough
- `alpha-auto-tech-film.mp4` — the "Stop Renting. Start Owning." video
- `alpha-auto-tech-overview.m4a` — the audio deep-dive
- `server.js` — zero-dependency static server (for Railway)
- `package.json` / `railway.json` — Railway build + start config

## Run locally

```
npm start
```

Serves on `http://localhost:3000` (or the `PORT` env var).

## Deploy (Railway)

Connected to Railway via this GitHub repo. Every push to `main` auto-deploys.
Railway reads `railway.json` (Nixpacks) and runs `npm start` → `server.js`.

Custom domain: **alphaauto.tech**

## Edit workflow

1. Edit `index.html` (or swap media in `slides/`, the `.mp4`, the `.m4a`)
2. `git add . && git commit -m "what changed" && git push`
3. Railway auto-deploys in ~1 minute

## Notes

- The video (~16MB) lives in the repo. If it changes often, move it to a CDN/YouTube and embed to keep the repo lean.
- Internal documents and source decks are intentionally **not** tracked here (see `.gitignore`).
