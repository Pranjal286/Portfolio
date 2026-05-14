# Pranjal Patel — Portfolio

A single-file, colorful, animated portfolio for an AI/ML engineer. No build step.

## Run locally

```bash
# from this folder
python3 -m http.server 8080
# open http://localhost:8080
```

## Add your profile photo

Your HEIC photo needs a one-time conversion. On macOS, run this in Terminal:

```bash
sips -s format jpeg ~/Downloads/IMG_3706.heic --out ./assets/profile.jpg --resampleHeightWidthMax 800
```

If `profile.jpg` is missing the page automatically falls back to a "PP" initials avatar with a rotating gradient ring.

## Deploy to GitHub Pages

```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/Pranjal286/portfolio.git
git push -u origin main
```

Then in the repo on github.com:

1. **Settings → Pages**
2. **Build and deployment → Source: Deploy from a branch**
3. **Branch:** `main` / **Folder:** `/ (root)` → **Save**

Your site goes live at `https://Pranjal286.github.io/portfolio/` in about a minute.

### Deploy to Vercel (alternative, like the reference site)

1. Push the repo to GitHub
2. Go to [vercel.com/new](https://vercel.com/new), import the repo
3. Framework preset: **Other** · Root directory: `./` · click Deploy

Vercel will give you a `*.vercel.app` URL immediately. You can attach a custom domain in **Project Settings → Domains**.

## Customizing

All content (text, links, projects) lives directly in `index.html`. Search for:

- `Pranjal286` — replace with your GitHub username if it changes
- `github.com/Pranjal286/credit-risk-scoring` — your fintech project repo
- `github.com/Pranjal286/clinical-rag-assistant` — your medical project repo
- Project cards live under `<!-- ===== PROJECTS ===== -->`

## Files

```
portfolio/
├── index.html        # everything — HTML + CSS + JS in one file
├── README.md         # you are here
└── assets/
    └── profile.jpg   # add your photo here (auto-detected)
```
