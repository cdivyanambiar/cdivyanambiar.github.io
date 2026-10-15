# personal-site

Static portfolio site (plain HTML/CSS/JS — no build step). Open `index.html` directly in a browser to preview locally.

## Deploy to GitHub Pages (user site: `<username>.github.io`)

1. On GitHub, create a **new repository** named exactly `<your-username>.github.io` (replace with your actual GitHub username, all lowercase). It must match exactly or Pages won't serve it at the root domain.
2. In this folder, initialize git and push the contents of `personal-site/` as the **root** of that new repo:
   ```powershell
   cd personal-site
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```
3. On GitHub: repo **Settings → Pages** → Source: `Deploy from a branch` → Branch: `main` / `(root)` → Save.
4. Wait a minute, then visit `https://<your-username>.github.io`.

## Editing content

- Text/sections: edit `index.html`.
- Colors/layout: edit `style.css` (CSS variables at the top control the color scheme).
- No profile photo is included — drop one in this folder (e.g. `photo.jpg`) and reference it in `index.html` if you want one.

## Custom domain (optional)

Add a `CNAME` file in this folder containing just your domain (e.g. `example.com`), then configure DNS per [GitHub's custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).
