# Portfolio Web Deployment

This is a static portfolio website ready for deployment.

## Deploy from Git to Vercel

### 1. Push the project to GitHub

If you do not already have a Git repository, run:

```bash
cd c:\Users\JOY ANGELIE NIEVES\OneDrive\Desktop\Mga Eme\HBO-ELEC 3\Documents\portfolio.web
git init
git add .
git commit -m "Initial portfolio site"
```

Then create a GitHub repository and add it as the remote:

```bash
git remote add origin https://github.com/<your-username>/<repo-name>.git
git branch -M main
git push -u origin main
```

### 2. Import into Vercel

1. Go to https://vercel.com and log in.
2. Click **New Project**.
3. Choose your Git provider (GitHub, GitLab, or Bitbucket).
4. Select the repository containing this portfolio.
5. If your site is in a subfolder, set the **Root Directory** to `portfolio.web`.
   - If the repository is only this folder, leave it as `.`.
6. Use the default settings for a static HTML site.
7. Click **Deploy**.

### 3. Deploy with Vercel CLI (optional)

If you prefer CLI deployment:

```bash
npm install -g vercel
cd c:\Users\JOY ANGELIE NIEVES\OneDrive\Desktop\Mga Eme\HBO-ELEC 3\Documents\portfolio.web
vercel login
vercel
```

For a production deploy:

```bash
vercel --prod
```

### 4. Confirm your site

- Make sure the repository contains `index.html` at the root.
- Make sure `assets/css/styles.css` and `assets/js/script.js` exist.
- Confirm Vercel deploys a static site successfully.

## Notes

- `portfolio.html` is kept as a backup, but Vercel will use `index.html` as the entry point.
- No build step is required because this is a static HTML/CSS/JS site.
