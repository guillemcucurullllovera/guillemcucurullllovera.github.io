# Guillem Cucurull Llovera — Personal Portfolio

A single-page, dark-themed portfolio site for Data Scientist / ML Engineer / Quant Researcher / Applied AI roles. Static HTML/CSS/JS — no build step, no backend.

## Contents

```
personal/
├── index.html                       # the entire site (self-contained)
├── favicon.svg                      # browser-tab icon (GC monogram)
├── robots.txt                       # allows search engines to index the page
└── assets/
    ├── logos/                       # affiliation logos (white silhouettes)
    └── writings/                    # downloadable PDF write-ups
        ├── CV_Guillem_Cucurull_Llovera.pdf
        ├── Quantum_ML_Multi_Asset.pdf
        └── AI_Hedge_Fund_Methodology.pdf
```

Everything the page needs is inside this folder. To work, the whole `personal/` folder must be deployed together (the page links to the logos and the PDFs by relative path).

## Preview locally

Just open `index.html` in a browser, or serve the folder:

```bash
cd personal
python3 -m http.server 8000
# then open http://localhost:8000
```

## Publish it (pick one — all free)

### Option A — Netlify Drop (fastest, ~60 seconds, no account needed to start)
1. Go to https://app.netlify.com/drop
2. Drag the entire `personal` folder onto the page.
3. You get a live URL instantly (e.g. `https://your-name.netlify.app`). Share it.
4. (Optional) Create a free account to rename the site or attach a custom domain.

### Option B — GitHub Pages (best if you want a permanent, versioned home)
1. Create a new GitHub repo (e.g. `portfolio`).
2. Upload the **contents** of this `personal` folder to the repo root (so `index.html` is at the top level).
3. Repo **Settings → Pages → Build and deployment**: Source = "Deploy from a branch", Branch = `main`, folder = `/ (root)`. Save.
4. Your site goes live at `https://<your-username>.github.io/portfolio/` within a minute or two.

### Option C — Vercel / Cloudflare Pages
Import the repo (or drag the folder) and deploy as a static site — no framework, root directory, no build command.

## Custom domain (optional)
All three hosts let you point a domain like `guillemcucurull.com` at the site for free (you only pay the domain registrar). Add it in the host's domain settings and follow their DNS instructions.

## Editing
Open `index.html` and edit directly — all content, styles and scripts are in that one file. The downloadable PDFs live in `assets/writings/`; replace them in place to update them.
