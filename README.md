# SINYU Sanitary Ware — Cloudflare Pages site

Static B2B catalog. Upload files to the root of `xybathware-bot/sinyu-bathware` on GitHub. Cloudflare Pages auto-deploys from `main` (framework None, build command blank, output directory root).

## Product editing
Edit `products.json` in GitHub. Every product requires unique `id`, `name`, `category`, `model`, `material`, `finish`, `description`, `image`. Categories: Faucets, Showers, Bidet Sprayers, Accessories, Drains & Fittings. For photos, upload compressed images to `assets/`, then set `image` to `/assets/filename.webp`. Avoid private information.

## Inquiries — setup needed
The form currently **does not send inquiries**. Edit `script.js` and set `CONTACT_EMAIL` to your verified company email to enable `mailto:` drafts. The buyer must send the email from their email app. For real server-side inquiry capture, configure a form service or Cloudflare Worker and privacy safeguards separately.

## Admin — setup needed
`/admin/` is an informational landing page, **not an authenticated visual CMS**. GitHub editing works now; Decap CMS requires a GitHub OAuth backend and data modeling, and should only be enabled after authentication is configured and tested. No credentials should be committed.

## Deployment
This package replaces the demo index.html. Upload all files preserving folder structure. Keep DNS unchanged until the site is verified. Placeholder products are examples, not claims of inventory or specifications.
