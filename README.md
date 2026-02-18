# Websites

Static websites deployed via Cloudflare Pages.

## Sites

### gavinrouse.com
Personal landing page — single-page HTML with dark theme.

**Deploy:**
1. Push to this repo
2. Cloudflare Pages auto-deploys from `gavinrouse.com/` directory
3. Custom domain: gavinrouse.com

## Structure
```
websites/
├── gavinrouse.com/
│   ├── index.html
│   └── README.md
└── README.md (this file)
```

## Cloudflare Pages Setup

1. Go to https://dash.cloudflare.com
2. Pages → Create a project
3. Connect to GitHub: `FranklinClawdbot/websites`
4. Configure:
   - **Project name:** gavinrouse-com
   - **Production branch:** master
   - **Build command:** (empty)
   - **Build output directory:** gavinrouse.com
5. Add custom domain: gavinrouse.com
