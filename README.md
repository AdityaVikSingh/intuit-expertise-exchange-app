# Intuit Expertise Exchange — clickable prototype

A real, static HTML/CSS site (no build step, no framework) covering the full flow:

- `index.html` — landing / role picker
- `exchange.html` — CFO marketplace of certified agents
- `agent.html` — agent trust & guardrails detail (Multi-Entity Close Copilot)
- `dashboard.html` — CFO's live IES dashboard after install
- `studio.html` — Agent Studio, where the advisor builds the agent
- `earnings.html` — advisor's earnings and installed-client view

Two flows, cross-linked exactly like the case's brief asks for: finance leader (index → exchange → agent → dashboard) and advisor (index → studio → earnings).

## Deploy to Vercel (one command)

You'll need a free Vercel account. From inside this folder:

```bash
npx vercel --prod
```

Follow the prompts (log in, confirm the project name, accept the defaults — it's a static site, no build command needed). Vercel will give you a live `https://...vercel.app` URL in under a minute. Paste that URL on your deck's cover slide.

To redeploy after an edit, just run `npx vercel --prod` again from this folder.

## Alternative: GitHub → Vercel dashboard

1. Create a new empty repo on GitHub.
2. From this folder:
   ```bash
   git remote add origin <your-repo-url>
   git push -u origin main
   ```
3. On vercel.com → **Add New Project** → **Import** your repo → **Deploy** (no config needed, it auto-detects a static site).

## Preview locally

Just double-click `index.html`, or run a tiny local server:

```bash
npx serve .
```
