# DSHBRD

Personal dashboard. Currently: BE transit board (`index.html`). More widgets coming.

Static site, no build step. Vercel serves `index.html` as-is.

## Local editing

Open the `DSHBRD` folder in VS Code. Edit `index.html` directly, then just open the file in a browser to preview (double-click it, or use the VS Code "Live Server" extension for auto-reload).

## Push to GitHub (one-time setup)

1. Go to github.com → New repository → name it `dshbrd` → **do not** add a README (you already have one) → Create.
2. In this folder, run:
   ```
   git init
   git add .
   git commit -m "init"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/dshbrd.git
   git push -u origin main
   ```

## Connect to Vercel for auto-deploy

Once it's on GitHub, tell Claude "connect the dshbrd repo to Vercel" — it'll link the repo so every push to `main` deploys automatically. No dashboard clicking needed.

(A first version is already live at a manual deployment; connecting GitHub replaces that with proper continuous deploys.)

## Adding more pages/widgets later

Keep it flat and simple: `life-dashboard.html`, `feed.html`, etc. next to `index.html`, or link them from `index.html` once there's more than one. Cross that bridge when it's actually needed, not before.
