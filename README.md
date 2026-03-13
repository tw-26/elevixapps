# Elevix Apps – Website

Static marketing site for the Elevix Apps monday.com app. Built with HTML, CSS, and JavaScript (Tailwind via CDN). Ready for **GitHub Pages**.

## Structure

| Path | Description |
|------|-------------|
| `/` or `index.html` | Landing page |
| `/docs/` or `/docs/getting-started.html` | Documentation |
| `/pricing` or `pricing.html` | Pricing |
| `/support` or `support.html` | Support (redirect to Tally when configured) |
| `/privacy` or `privacy.html` | Privacy policy |
| `/monday-app-association.json` | monday.com app association file |

## GitHub Pages

1. Push this repo to GitHub.
2. **Settings → Pages** → Source: **Deploy from a branch**.
3. Branch: `main` (or `master`), folder: **/ (root)**.
4. Save. The site will be at `https://<username>.github.io/<repo>/`.

For a custom domain, set it in Pages settings and add a `CNAME` file with the domain.

## Before going live

1. **monday.com app association**  
   Edit `monday-app-association.json` and replace `YOUR_CLIENT_ID` with your app’s client ID.

2. **Support / Tally**  
   In `support.html`, set `TALLY_FORM_URL` to your Tally form URL (e.g. `https://tally.so/r/xxxxx`).

3. **Content**  
   Replace placeholder copy and images with your real app name, screenshots, and links.

## Local preview

Open `index.html` in a browser, or use a simple server:

```bash
npx serve .
```

Then visit `http://localhost:3000` (or the port shown).
