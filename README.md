# Portfolio site

Static site: `index.html` + `styles.css`. No build step needed.

## Publish on GitHub Pages

1. Create a new repository named `your-username.github.io` (replace with your actual GitHub username) — this exact naming makes GitHub serve it as your main Pages site. If you'd rather keep it as a project inside an existing repo, any repo name works too.
2. Upload `index.html`, `styles.css`, and (once you have one) `resume.pdf` to the repository root.
3. Go to the repo's **Settings → Pages**, set the source branch to `main` (or `master`) and folder to `/root`, then save.
4. Your site will be live at `https://your-username.github.io` (or `https://your-username.github.io/repo-name` for a project repo) within a few minutes.

## Before you publish, update these placeholders in `index.html`

- `your.email@example.com` → your real email
- `https://www.linkedin.com/in/your-profile` → your LinkedIn URL
- `https://github.com/your-username` → your GitHub profile URL
- `resume.pdf` → upload your actual resume PDF with this filename, or update the link

## Adding real dashboard screenshots or embeds

Each project block in `index.html` (`<article class="project">`) currently has text only. To add an image, drop it in the folder and add, e.g.:

```html
<img src="esg-dashboard.png" alt="ESG disclosure dashboard screenshot" style="width:100%; margin-top:16px; border:1px solid var(--hairline);">
```

To embed a live Power BI "Publish to web" or Tableau Public dashboard instead of a static image, use an `<iframe>` with the embed URL each platform gives you.
