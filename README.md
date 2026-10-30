# eliskagreplova.com

Personal site. Plain HTML + CSS, hosted free on GitHub Pages from the
`gh-pages` branch of `greplova/greplova.github.io`.

- `index.html` — the main page
- `reading.html` — reading list
- `style.css` — the look; colors are at the top (`--bg`, `--heading`, `--accent`)
- `photo.jpg` — portrait

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Publish changes

```bash
git add .
git commit -m "Describe the change"
git push
```

GitHub rebuilds the site a minute or two after each push.
Live at https://greplova.github.io

## Use your own domain (eliskagreplova.com)

1. On GitHub: **Settings → Pages → Custom domain**, enter `www.eliskagreplova.com`, Save.
2. At your domain registrar's DNS settings:
   - Remove the old Google Sites records.
   - Add a `CNAME` record: host `www` → `greplova.github.io`
   - Add four `A` records for the bare domain (`@`):
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. In Google Sites, remove the custom domain from the old site.
4. Once DNS has updated (minutes to a few hours), tick **Enforce HTTPS** in GitHub Pages settings.
