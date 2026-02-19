# Cloudflare Pages Deployment

## gavinrouse.com

Static single-page HTML site deployed via Cloudflare Pages.

### Structure
```
sites/gavinrouse.com/
└── index.html    # Main landing page
```

### Deployment Steps

1. **Go to Cloudflare Dashboard**
   - https://dash.cloudflare.com
   - Sign in with your Cloudflare account

2. **Navigate to Pages**
   - Click "Pages" in the left sidebar
   - Click "Create a project"

3. **Connect to GitHub**
   - Select "Connect to GitHub"
   - Authorize Cloudflare to access your repos
   - Select: `FranklinClawdbot/franklin-openclaw-workspace`

4. **Configure Build Settings**
   - **Project name:** gavinrouse-com
   - **Production branch:** master
   - **Build command:** (leave empty - static site)
   - **Build output directory:** sites/gavinrouse.com
   - Click "Save and Deploy"

5. **Add Custom Domain**
   - After initial deploy, go to project settings
   - Click "Custom domains" tab
   - Click "Set up a custom domain"
   - Enter: gavinrouse.com
   - Follow DNS verification steps (add CNAME record)

### Updating the Site

1. Edit files in `sites/gavinrouse.com/`
2. Commit and push to GitHub
3. Cloudflare Pages auto-deploys on every push to master

### Current Site

- **Tagline:** Engineer. Builder. Free Man.
- **Location:** Pasco, Washington
- **Features:** Responsive design, dark theme, contact links

### DNS Configuration (Required)

In your Cloudflare DNS settings for gavinrouse.com:

```
Type: CNAME
Name: @ (or www)
Target: gavinrouse-com.pages.dev
TTL: Auto
Proxy: Enabled (orange cloud)
```

Or use the Cloudflare Pages automatic DNS setup during custom domain configuration.
