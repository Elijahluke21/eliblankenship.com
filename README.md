# eliblankenship.com

Personal site for Eli Blankenship: a home hub with Bible maps, a blog, resources, and an about page.

Plain static HTML and CSS. No build step: every folder with an `index.html` is a page.

```
index.html                 Home (chart index)
assets/css/site.css        Shared styles and color tokens (light + dark)
maps/index.html            Maps gallery, grouped by era
maps/<map-name>/index.html One self-contained interactive map per folder
blog/  resources/  about/  Section pages
404.html                   Not-found page (served automatically by Netlify)
netlify.toml               Netlify settings (no build step, www → bare domain)
favicon.svg                Sailboat mark
```

## Adding a map

1. Create `maps/<map-name>/index.html` (a self-contained page).
2. Add a card for it in `maps/index.html` under the right era.
3. Commit and push. The site redeploys automatically.

## Hosting

Hosted on Netlify, connected to this repo. Every push to `main` redeploys automatically.

- Build command: *(none)*
- Publish directory: `.` (set in `netlify.toml`)

Domain: `eliblankenship.com` is registered at GoDaddy. DNS records point to Netlify.
