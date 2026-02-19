# Gavin Rouse — The Rouse House

Personal website.

## Structure

```
gavinrouse/
├── index.html    # Main landing page
└── README.md     # This file
```

## Current Deployment

- **Host:** GitHub Pages
- **URL:** https://franklinclawdbot.github.io/websites/gavinrouse/

## End Goal: Cloudflare Pages

### Setup

1. **Go to Cloudflare Dashboard** → Pages → Create project
2. **Connect to GitHub** → Select `FranklinClawdbot/websites`
3. **Configure:**
   - Project name: `gavinrouse-com`
   - Production branch: `master`
   - Build command: *(empty - static site)*
   - Build output directory: `built-site/gavinrouse`
4. **Add Custom Domain:** gavinrouse.com

### DNS (when ready)

```
Type: CNAME
Name: @
Target: gavinrouse-com.pages.dev
```

### Updating

1. Edit `built-site/gavinrouse/index.html`
2. Commit and push
3. Auto-deploys

## Site Info

- **Tagline:** Engineer by trade. Builder by nature.
- **Location:** Pasco, Washington
- **Theme:** Cormorant Garamond + DM Sans