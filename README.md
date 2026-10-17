# Rishab Advani, portfolio site

One static page. No build step and no dependencies. The site lives in `public/`; `vercel.json` tells Vercel to serve that folder and adds a few security headers.

## Deploy on Vercel

**Option 1: Vercel CLI** (needs Node.js)

1. `npm i -g vercel`
2. In this folder run `vercel`. Log in when asked, accept the defaults, and name the project (for example `rishab-advani`). This creates a preview deployment.
3. Run `vercel deploy --prod`. The production URL is `https://<project-name>.vercel.app`.

**Option 2: Git** (every push redeploys automatically)

1. Push this folder to a GitHub repository, with `vercel.json` and `public/` at the top level.
2. Go to vercel.com/new, import the repository, leave Framework Preset as **Other** and Build Command blank, then click Deploy.

Share the production URL, not the preview URL. With Vercel's default settings, preview and per-deployment URLs ask visitors to log in; the production domain is public.

## Edit

- Text and layout: `public/index.html`
- Photo in colour instead of black and white: in the `<style>` block at the top of `public/index.html`, change `--photo-filter` to `none`
- Resume: replace `public/assets/Rishab_Advani_Resume.pdf` and keep the file name. The PDF is publicly downloadable once deployed, so check what it contains (it includes a phone number). To remove it, delete the file and the "Resume (PDF)" link near the end of `index.html`.
- Fonts (Newsreader and Instrument Sans) load from Google Fonts.
