# Drishti — Landing Page

## Deploy to GitHub Pages with custom domain

1. Create a public repo on GitHub named `drishti`
2. Push these files to the `main` branch
3. Go to Settings → Pages → Source → select `main` branch, root folder
4. Under "Custom domain", enter `climate-drishti.store` and save
5. Check "Enforce HTTPS" once the DNS check passes

## DNS setup (in your domain registrar)

Add these records where you bought the domain:

| Type  | Host/Name | Value                          |
|-------|-----------|--------------------------------|
| A     | @         | 185.199.108.153                |
| A     | @         | 185.199.109.153                |
| A     | @         | 185.199.110.153                |
| A     | @         | 185.199.111.153                |
| CNAME | www       | YOURUSERNAME.github.io         |

Replace YOURUSERNAME with your GitHub username.

DNS propagation usually takes 5–30 minutes. Once it's done, your site will be live at https://climate-drishti.store

## Files

- `index.html` — Full landing page (single file, no build step)
- `CNAME` — Tells GitHub Pages your custom domain
- `.nojekyll` — Skips Jekyll processing
