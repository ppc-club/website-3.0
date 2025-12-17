# PPC Club Website (Chulapa/Jekyll) — drop-in bundle

## 1) Copy files into your repo

Copy the contents of this folder into the root of your `ppc-club/website-3.0` repo:

- `_data/meetups.yml`
- `_pages/*.md`
- `index.md`
- `assets/css/ppc.css`

## 2) Ensure pages are built

Most Jekyll setups will automatically build `_pages` if your theme supports it. If your Chulapa config doesn’t, move the page files into the root (e.g. `meetups.md` with `permalink: /meetups/`).

## 3) Load the CSS

How you add CSS depends on your Chulapa layout. Options (pick the one that matches your theme):

### Option A (recommended): add to your head include
Look for a file like `_includes/head.html` and add:

```html
<link rel="stylesheet" href="{{ '/assets/css/ppc.css' | relative_url }}">
```

### Option B: add via config
Some themes allow adding `custom_css` in `_config.yml`. If yours does, point it to `assets/css/ppc.css`.

## 4) Update the schedule
Edit `_data/meetups.yml` and you’re done.

## 5) Merch link
Right now merch points at Etsy: https://www.etsy.com/shop/ProspectParkChess

When you kill Etsy, replace the URL on `/merch/` and `/links/`.
