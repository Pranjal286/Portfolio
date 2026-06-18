# Pranjal Patel — Portfolio

Single-file, colorful portfolio for an AI/ML and full‑stack engineer — no build step, just HTML + CSS + JS.

This site highlights my experience in fraud and risk modeling, RAG systems, and ML applications in fintech and healthcare.

## Run locally

```bash
# from this folder
python3 -m http.server 8080
# open http://localhost:8080
```

## Profile photo

Add your profile photo at:

```text
./assets/profile.jpg
```

If `profile.jpg` is missing, the page falls back to a “PP” initials avatar with a rotating gradient ring.

## Deploy

You can host this portfolio either on GitHub Pages or Vercel.

### GitHub Pages

```bash
git init
git add .
git commit -m "Portfolio"
git branch -M main
git remote add origin https://github.com/Pranjal286/Portfolio.git
git push -u origin main
```

Then on github.com:

1. Go to **Settings → Pages**
2. Under **Build and deployment**, set **Source: Deploy from a branch**
3. Choose **Branch:** `main` and **Folder:** `/ (root)` → **Save**

Your site will be live at a URL like:

```text
https://Pranjal286.github.io/Portfolio/
```

### Vercel

1. Push this repo to GitHub
2. Go to [https://vercel.com/new](https://vercel.com/new) and import the repo
3. Framework preset: **Other** · Root directory: `./` · click **Deploy**

Vercel will give you a `*.vercel.app` URL. You can attach a custom domain from **Project Settings → Domains**.

## Customizing content

All text (about, skills, experience, projects, contact) lives directly in:

```text
index.html
```

Look for these sections inside the file:

- `<!-- ===== ABOUT ===== -->` to adjust the summary and quick facts
- `<!-- ===== SKILLS ===== -->` to tweak chips / tools
- `<!-- ===== EXPERIENCE ===== -->` for BlackRock and Cred experience including internship
- `<!-- ===== PROJECTS ===== -->` for Morph & Split, Brain Tumor Segmentation, Credit Risk and RAG projects
- `<!-- ===== CONTACT ===== -->` for email, phone, LinkedIn, GitHub

## Files

```text
Portfolio/
├── index.html        # everything — HTML + CSS + JS in one file
├── README.md         # this file
└── assets/
    └── profile.jpg   # optional profile image (auto-detected)
```
