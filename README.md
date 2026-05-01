# RETAIN Main Landing Page

Main landing page for retain.co.id — umbrella brand for ROASlab and Chatback products.

## Products
- **ROASlab**: AI ads decision tool for Shopee sellers → [roaslab.retain.co.id](https://roaslab.retain.co.id)
- **Chatback**: CRM chat blast tool → [chatback.retain.co.id](https://chatback.retain.co.id)

## Tech Stack
- HTML + Tailwind CDN + Custom CSS tokens
- Deployed via Cloudflare Workers & Pages

## Development
```bash
# Open index.html in browser for local preview
open index.html
```

## Deployment

### Cloudflare Workers & Pages

This project is deployed via Cloudflare Workers & Pages with automated GitHub pipeline.

#### Setup (One-time)
1. Connect this repo to Cloudflare Pages: `dash.cloudflare.com` → Workers & Pages → Create → Pages → Connect to Git
2. Select repository: `naufalazhr/retain-main-LP`
3. Build settings:
   - Framework preset: **None**
   - Build command: *(leave empty)*
   - Build output directory: `.`
4. Set custom domain: `retain.co.id` in Cloudflare dashboard → Custom domains

#### Manual Deploy (via Wrangler CLI)
```bash
# Install Wrangler CLI
npm install -g wrangler

# Login to Cloudflare
wrangler login

# Deploy
wrangler pages deploy . --project-name=retain-main-lp
```

#### Auto-Deploy
Push to `main` branch triggers automatic deployment via Cloudflare GitHub integration.
