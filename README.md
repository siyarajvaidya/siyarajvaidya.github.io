# Kindroots Websites

Three static sites, one family. Ready for GitHub Pages (free hosting).

## What's here

- `/` — **Kindroots Foundation** (parent site): `index`, `our-story`, `programs`, `impact`, `get-involved`, `news`
- `/share-and-care/` — **Share & Care** program site: `index`, `what-we-make`, `who-we-help`, `volunteer`, `news`
- `/treats-for-tails/` — **Treats for Tails** redesign: `index`, `our-mission`, `what-we-make`, `impact`, `get-involved`
- Each site has its own stylesheet at `assets/css/style.css`. All links are relative, so the whole folder deploys as one unit.

## Deploy to GitHub Pages (free)

1. Create a new public repo on GitHub (e.g. `kindroots`).
2. Unzip this folder and push it:
   ```
   cd kindroots-websites
   git init
   git add .
   git commit -m "Kindroots family sites v1"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/kindroots.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main`, folder: `/ (root)`. Save.
4. Live in about a minute at `https://YOUR-USERNAME.github.io/kindroots/`
   - Share & Care: `.../kindroots/share-and-care/`
   - Treats for Tails: `.../kindroots/treats-for-tails/`

## Custom domain (later, ~$15/year)

Buy `kindroots.org` (or similar) from any registrar. In the repo's **Settings → Pages**, add it as the custom domain and add the DNS records GitHub shows you. The sub-paths keep working unchanged.

## Updating the sites

Edit any `.html` file, commit, push — GitHub Pages redeploys automatically within a minute or two. This loop works great with Codex on your Mac: describe the change, review the diff, push.

News posts are plain HTML sections with real dates — to add one, copy an existing post block, change the date and text.

## Before launch checklist

- [ ] Replace `[PHOTO: ...]` placeholders with real photos (pillows, tags, volunteers, deliveries)
- [ ] Verify donation counts — search the HTML for `TODO`
- [ ] Decide the fate of the old Google Sites Treats for Tails page (keep live until launch, then unpublish or redirect)
- [ ] Optional: add `sitemap.xml` / `robots.txt` if search visibility matters
