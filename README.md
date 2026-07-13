# Ricardo Martinez-Garcia — Group Website

Static site, no build step required. Six pages plus an `images/` folder of local assets — everything is linked with relative paths, so it works as-is on GitHub Pages, Netlify, Vercel, or any plain static host.

## Files

```
index.html          About (home page)
research.html        Research
publications.html    Publications
team.html             Team (includes the interactive world map)
teaching.html         Teaching
news.html              News
images/                 Logo, banner, and team/portrait photos
```

## Publish with GitHub Pages (recommended)

1. Create a new repository on GitHub.
   - If you want the site at `https://rmtzgarcia.github.io` directly, name the repo exactly `rmtzgarcia.github.io`.
   - Otherwise, name it anything (e.g. `lab-website`) and it'll be served at `https://rmtzgarcia.github.io/lab-website/`.
2. Upload the contents of this `site` folder to the repo root — keep `index.html` and the other `.html` files at the top level, and keep the `images` folder alongside them (don't nest them in a subfolder).
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to "Deploy from a branch", branch `main`, folder `/ (root)`.
5. Save. GitHub will give you a live URL within a minute or two (visible at the top of the Pages settings page).

## Custom domain (optional)

If you want a domain like `ricardomartinezgarcia.com` instead of the `github.io` address, buy the domain from any registrar, then in the same **Settings → Pages** panel enter it under "Custom domain." GitHub will show you the DNS records to add at your registrar (usually a couple of `A` records or a `CNAME`). It can take up to 24 hours to propagate.

## After it's live

- Update the link on your Google Scholar profile, CASUS/HZDR group page, and CV to point to the new URL.
- Consider adding a short "moved" notice on the old Google Sites page (`sites.google.com/view/rmtzgarcia`) linking to the new site, so old bookmarks and search results aren't dead ends.

## Notes

- All photos and the logo are stored locally in `images/` — nothing depends on Google's servers, so there's no risk of broken images from expired links.
- The `.person` photos for Timon Althaus, Zihao Liu, and Khaled Yasein currently show initials instead of a real photo (no photo was available for them at build time). Drop a real photo into `images/` and update the relevant `<img>` tag in `team.html` if that changes.
