# whistleravenandfootnote.com

The static website for **Whistle, Raven & Footnote LLC**, served by GitHub Pages at
<https://whistleravenandfootnote.com>.

## Files

| Path | Purpose |
|---|---|
| `index.html` | Home page (single page) |
| `styles.css` | All styles |
| `404.html` | Not-found page |
| `assets/` | Logo (dark and light), raven mark, favicons, social share image |
| `CNAME` | Custom domain for GitHub Pages |
| `.nojekyll` | Tells Pages to serve the files as they are |

No build step. To preview locally: `python -m http.server 8000` then open http://localhost:8000.

## Deploying (GitHub Pages)

1. Push to `main` on `drpaj12/whistle-raven-AND-footnote`.
2. Repo **Settings → Pages**: Source = *Deploy from a branch*, Branch = `main`, folder `/ (root)`.
3. Custom domain: `whistleravenandfootnote.com` (picked up from `CNAME`). Tick **Enforce HTTPS** once the certificate is issued.
4. DNS at your registrar:
   - `A` records for `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `AAAA` records for `@` (optional) → `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`
   - `CNAME` for `www` → `drpaj12.github.io`
