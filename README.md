# AI Advantage Learnings

A 14-day course distilled from 14 months of AI Advantage Club content. Three views: a curriculum to walk day by day, a knowledge base to search, cheat sheets to grab and go.

## Open it locally

Open `index.html` in any modern browser. Done. No build step, no dependencies.

## Deploy to GitHub Pages (recommended)

Two ways. Pick the easier one.

### Option A — GitHub web UI (no command line)

1. Go to github.com → click **New repository**.
2. Name it whatever you want — for example `ai-learnings` or `aia-course`. Set it to **Public**. Don't initialize with a README (you already have one).
3. On the new empty repo page, click **uploading an existing file**.
4. Drag these five files in:
   - `index.html`
   - `styles.css`
   - `app.js`
   - `data.js`
   - `.nojekyll`
   (You can optionally include `README.md` too.)
5. Click **Commit changes**.
6. Go to **Settings → Pages** in the repo.
7. Under **Source**, pick **Deploy from a branch**.
8. Set branch to `main`, folder to `/ (root)`. Click **Save**.
9. Wait ~30–60 seconds. GitHub will show your live URL at the top of the Pages settings — something like `https://YOURUSERNAME.github.io/ai-learnings/`.

### Option B — From your terminal

```bash
cd ai-advantage-learnings
git init
git add .
git commit -m "Initial commit"
gh repo create ai-learnings --public --source=. --push
```

Then go to **Settings → Pages** on the new repo, set Source to `main` / `/ (root)`, click **Save**.

## Updating later

To add new content: edit `data.js` (for Knowledge Base or Tool Stack items), or edit `index.html` (for new curriculum lessons or cheat sheets). Commit and push — Pages rebuilds automatically.

## Other deploy options

It's a static site (HTML, CSS, JS — no framework, no build). Drop the folder anywhere static hosting works:

- **Netlify** — drag the folder onto netlify.com/drop. Live URL in 30 seconds.
- **Vercel** — `vercel deploy` from the folder, or drag-and-drop in the dashboard.
- **Cloudflare Pages** — `wrangler pages deploy .` or drag-and-drop in the dashboard.
- **Your own server** — copy the five files (`index.html`, `styles.css`, `app.js`, `data.js`, `.nojekyll`) to any web root.

## Files

```
ai-advantage-learnings/
├── index.html      # the site
├── styles.css      # all styling
├── app.js          # tabs, search, copy buttons, progress tracking
├── data.js         # the knowledge base + tool stack content
├── .nojekyll       # tells GitHub Pages to skip Jekyll processing
└── README.md
```

## What's covered

- Curriculum: 14 daily modules (64 lessons total) walking from prompting basics through the operator-pattern tools (Claude Cowork, Skills) and the expert-series mindset work. Do one a day, or knock out a few on a weekend.
- Knowledge Base: ~65 distilled topics across Foundations, Workflow, Content, Research, Visuals, Ops, and Mindset.
- Cheat Sheets: the 5-block prompt template, the reusable playbook method, the problem-first system, the reply library, the handoff prompt, and the tool-stack table.
- Tool Stack: every tool that came up across the 14 months, with purpose and notes.
- Expert Series: takeaways from Marie Forleo, Zack Kass, Amjad Masad, Sabrina Ramonov, plus the "irreplaceable strengths" workshop.

Progress (which lessons you've completed) is stored in your browser's localStorage. It survives reloads. It doesn't sync across devices.
