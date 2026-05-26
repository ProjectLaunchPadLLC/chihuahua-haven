# Chihuahua Haven

A small Chihuahua care website with articles, a local chatbot page, and Cloudflare Workers compatibility.

## Files

- `public/index.html` — homepage
- `public/bot.html` — local chatbot interface
- `public/posts/` — article pages for care, feeding, and barking tips
- `public/style.css` — shared visual styling
- `public/404.html` — not-found page
- `worker.js` — Cloudflare Worker script for serving static assets from `public`
- `wrangler.toml` — Cloudflare Worker site configuration

## Deploying with Cloudflare Workers

1. Install Wrangler: `npm install -g wrangler`
2. Authenticate: `wrangler login`
3. Deploy the site: `wrangler deploy --site`

## Deploying with Cloudflare Pages

1. Connect this repository in the Cloudflare Pages dashboard.
2. Set the build command to none.
3. Set the output directory to `public`.
4. Deploy.

## Notes

- The site is static and can be served directly from `public`.
- The Worker script is already configured to fetch assets from the public bucket.
- `public/index.html` is the home entry point for the site.
