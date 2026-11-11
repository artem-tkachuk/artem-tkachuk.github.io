# artem-tkachuk.github.io

Personal site. One `index.html`, no build step, no dependencies beyond Google Fonts.

## Edit

Each tile is a `<section class="tile">` or `<a class="tile">` inside `.grid`.

- `w2` makes a tile two columns wide, `h2` two rows tall.
- Colours and fonts are tokens in the `:root` block at the top of the `<style>`.
- Light and dark themes both come from those tokens.

## Preview locally

```sh
python3 -m http.server 8000
```

## Deploy

**GitHub Pages** (workflow included):

1. Create a repo named `<your-username>.github.io` and push `main`.
2. Repo Settings → Pages → Source: **GitHub Actions**.
3. Every push to `main` redeploys.

**Cloudflare Pages / Netlify / Vercel**: point at the repo, no build command, output directory `/`.
