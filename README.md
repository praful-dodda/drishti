# Drishti — Landing Page

## Before you deploy

1. **Find-and-replace** `YOURDOMAIN.com` with your actual domain (e.g., `drishtirisk.com`) in:
   - `index.html` (email addresses — there are 4 occurrences of `praful@YOURDOMAIN.com`)
   - `CNAME` (replace with just the bare domain, e.g., `drishtirisk.com`)

2. **Add your headshot** — Replace the "Your photo here" placeholder in the founder section with an actual `<img>` tag.

## Deploy to GitHub Pages

1. Create a new repo on GitHub (e.g., `drishti-site`)
2. Push these files to the `main` branch
3. Go to **Settings → Pages → Source** → select `main` branch, root folder
4. In your domain registrar (Namecheap, Cloudflare, etc.), add these DNS records:
   - `A` record pointing to `185.199.108.153`
   - `A` record pointing to `185.199.109.153`
   - `A` record pointing to `185.199.110.153`
   - `A` record pointing to `185.199.111.153`
   - `CNAME` record: `www` → `YOURUSERNAME.github.io`
5. Back in GitHub Pages settings, enter your custom domain and check "Enforce HTTPS"
6. Wait 5–15 minutes for DNS propagation

## Files

- `index.html` — The entire landing page (single file, no build step)
- `CNAME` — Tells GitHub Pages your custom domain
- `.nojekyll` — Skips Jekyll processing (faster deploys)
