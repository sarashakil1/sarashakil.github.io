# Portfolio

A single-file, no-build personal portfolio (marketing analytics & data engineering).
Everything lives in `index.html` — plain HTML and CSS, no framework, no compile step.

## Edit it

Open `index.html` and search for the word **EDIT**. Each spot is marked with a comment.
The order to work through:

1. `<title>` — your name
2. **Hero** — name, one-line positioning, intro, current role
3. **Results ledger** — your real numbers (or delete rows)
4. **About** and *What I do*
5. **Stack** — your tools
6. **Work** — projects; change each `href="#"` to a real case-study or repo link
7. **Experience** — your roles
8. **Contact** — email, résumé link, GitHub, LinkedIn

To preview locally, just double-click `index.html` — it opens in any browser.

## Publish free on GitHub Pages

1. Create a new **public** repo on GitHub.
   - Name it `yourusername.github.io` to get a clean root URL,
     or any name (e.g. `portfolio`) for a `/portfolio` path.
2. Push these files (see commands below).
3. On GitHub: **Settings → Pages → Build and deployment**.
   Set **Source: Deploy from a branch**, **Branch: `main` / `root`**, then **Save**.
4. Wait ~1 minute. Your site is live at the URL shown on that Pages screen.

### Push commands

```bash
cd path/to/this/folder
git init
git add .
git commit -m "Portfolio site"
git branch -M main
git remote add origin https://github.com/YOURUSERNAME/YOURREPO.git
git push -u origin main
```

Any time you edit, republish with:

```bash
git add . && git commit -m "Update" && git push
```

## Custom domain (optional)

Buy a domain, then in **Settings → Pages → Custom domain** enter it and follow the
DNS instructions GitHub shows. Add a file named `CNAME` containing just your domain.
