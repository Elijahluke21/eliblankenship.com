# eliblankenship.com

Personal site for Eli Blankenship: a home hub with Bible maps, a blog, resources, and an about page.

Plain static HTML and CSS. No build step: every folder with an `index.html` is a page.

```
index.html                 Home (chart index)
assets/css/site.css        Shared styles and color tokens (light + dark)
maps/index.html            Maps gallery, grouped by era
maps/<map-name>/index.html One self-contained interactive map per folder
blog/  resources/  about/  Section pages
404.html                   Not-found page (served automatically by Cloudflare Pages)
favicon.svg                Sailboat mark
```

## Adding a map

1. Create `maps/<map-name>/index.html` (a self-contained page).
2. Add a card for it in `maps/index.html` under the right era.
3. Commit and push. The site redeploys automatically.

## Hosting

Hosted on Cloudflare Pages, connected to this repo:

- Framework preset: **None**
- Build command: *(leave empty)*
- Build output directory: `/`

Domain: `eliblankenship.com` is registered at GoDaddy, with its nameservers pointed to Cloudflare.
