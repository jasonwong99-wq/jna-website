# J & A App Studio — company website

Live site: https://jnaappstudio.com (once the domain is connected)
Hosting: Cloudflare Pages, free. Every push to the `main` branch goes live in about a minute.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole homepage. Design, text and the three app sections are all in this one file. |
| `app-template.html` | Copy this to make a page for a new app (e.g. `pipo.html`). |
| `images/` | App icons (`mum-hero-icon.png`, `eldivo-icon.png`, `cukaisifu-icon.png`) and the studio logo: `logo-mark.svg/.png` (light), `logo-mark-dark.svg/.png`, `logo-lockup.svg/.png` (mark + wordmark), `app-icon.png` (1024, for store and social profiles), `favicon.svg`. Add new app icons here. |
| `README.md` | This file. |

Never put SSM documents, receipts or anything private in this folder: it is public on GitHub.

No build step, no WordPress, no database. Open `index.html` in a browser to preview.

## How to add a new app (about 30 minutes with Claude)

1. In `index.html`, find the `<!-- APP: CukaiSifu -->` block (the last `<article class="app ...">`).
2. Copy the whole block, paste it below, and change: name, status pill, description, 3–4 features, price, store links, and the phone mockup text.
3. Pick an accent colour: add two tokens in `:root` (e.g. `--pink` and `--pink-soft`) and a class like `.pipo{--dot:var(--pink)}`.
4. Change the hero line "3 apps in the family" to the new count.
5. Copy `app-template.html` to `<appname>.html` and fill it in.
6. Commit and push. Done.

## Publishing changes

```
git add .
git commit -m "Describe the change"
git push
```

Or just tell Claude what changed.

## Company details used on the site

J & A APP STUDIO PLT · 202604002661 (LLP0047906-LGN)
No. 123, Jalan Permata 1/KS09, Pusat Bandar Perniagaan Bandar Bestari,
Taman Perindustrian Air Hitam, 42000 Klang, Selangor, Malaysia
+60 12-213 0661 · jasonwong99@gmail.com (to be replaced by hello@jnaappstudio.com once the domain is live)
