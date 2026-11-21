# undefinedtoken.com

Personal site for **Ezaz Ansari** — designer in Bengaluru, currently Principal Product Designer at Upstox.

Live at: [undefinedtoken.com](https://undefinedtoken.com/)

## Stack

Single static HTML file. No build step, no framework.

- Type set in [Departure Mono](https://departuremono.com/) by Helena Zhang & Tobias Fried.
- Drawing canvas on the page (local only, nothing is sent anywhere).
- Full-page snapshot export via [html2canvas](https://html2canvas.hertzen.com/).

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole site — markup, styles, scripts, base64 avatar, all inline |
| `robots.txt` | Allows all major search and AI crawlers, points to sitemap |
| `sitemap.xml` | Single-URL sitemap for search engines |
| `llms.txt` | AI-crawler-friendly summary ([llmstxt.org](https://llmstxt.org/) spec) |
| `vercel.json` | Security headers (CSP, HSTS, frame protection) + caching for static assets |

## Local development

```bash
# Just open the file in a browser:
open index.html

# Or serve it locally so paths resolve like production:
npx serve .
```

## Deployment

Hosted on [Vercel](https://vercel.com). Pushing to `main` auto-deploys.

To run a manual deploy from the CLI:

```bash
npm i -g vercel
vercel --prod
```

## Features

- Draw on the page with a crayon cursor
- Subtle cursor trail follows the mouse even outside draw mode
- Avatar tilts with scroll velocity
- Konami code (↑↑↓↓←→←→BA) for chaos mode
- Page-snapshot PNG export
- Light theme with a hand-picked warm palette
- Designed dead-simple — small column, generous whitespace, single column on mobile

## Credits

Type by [Helena Zhang & Tobias Fried](https://github.com/rektdeckard/departure-mono).
