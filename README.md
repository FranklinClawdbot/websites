# gavinrouse.com

Personal website built with Hugo and PaperMod theme.

## Structure

- `content/about.md` — About page
- `content/projects.md` — Project portfolio
- `content/now.md` — Now page (current focus)
- `hugo.toml` — Site configuration
- `public/` — Generated static site (don't edit directly)

## Local Development

```bash
cd /home/gavin/.openclaw/workspace/websites/gavinrouse.com
hugo server -D
```

Visit http://localhost:1313

## Build for Production

```bash
hugo --minify
```

Output is in `public/` directory.

## Deployment Options

### Option 1: Cloudflare Pages (Recommended)
1. Push to GitHub
2. Connect repo to Cloudflare Pages
3. Build command: `hugo --minify`
4. Build output: `public`
5. Free, fast, automatic deploys

### Option 2: GitHub Pages
1. Push to GitHub
2. Enable GitHub Pages from repo settings
3. Use GitHub Actions workflow for Hugo builds

### Option 3: Self-hosted (Proxmox/NGINX)
1. Build: `hugo --minify`
2. Copy `public/` to web server directory
3. Configure NGINX to serve static files

### Option 4: Netlify
1. Push to GitHub
2. Connect to Netlify
3. Build settings auto-detected from `hugo.toml`

## Content Updates

Add new posts:
```bash
hugo new content posts/my-post.md
```

Edit existing pages in `content/` directory.

## Theme Updates

PaperMod theme is a git submodule:
```bash
git submodule update --remote themes/PaperMod
```

## TODO

- [ ] Add profile image
- [ ] Write first blog post
- [ ] Configure actual social links
- [ ] Set up deployment pipeline
- [ ] Add analytics (optional)
