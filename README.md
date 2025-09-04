# Marketing Dojo - GitHub Pages ready repo

This folder was generated automatically from the uploaded zip.

**Before pushing to GitHub:**  
- Replace the `CNAME` file's content (`yourdomain.com`) with your actual domain (e.g. `example.com` or `www.example.com`).  
- If you prefer a different branch or repo name, you can adjust GitHub Pages settings later.

## Quick push commands (example)

```bash
cd /path/to/this/folder
git init
git add .
git commit -m "Initial site"
# create repo on GitHub via web UI or using gh CLI:
# gh repo create <repo-name> --public --source=. --remote=origin --push
git remote add origin git@github.com:<your-username>/<repo-name>.git
git branch -M main
git push -u origin main
```

## GitHub Pages setup
1. In your repository on GitHub, go to **Settings → Pages**.
2. Select the branch `main` (root) as the publishing source and save.
3. Under **Custom domain**, enter your domain (without `http://`) and save.
4. Optionally enable "Enforce HTTPS" once GitHub provisions the certificate.

## DNS notes (do this in GoDaddy DNS settings)
- For an **apex/root domain** (example.com), add 4 A records for `@` to point to GitHub Pages IPs (see GitHub docs).
- For a **www** subdomain, add a CNAME record: `www` → `<your-username>.github.io`

See GitHub Docs for the authoritative steps:
https://docs.github.com/pages/configuring-a-custom-domain-for-your-github-pages-site