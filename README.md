# BlueCard website

Static site for the BlueCard card game app, published with GitHub Pages. No build step: plain HTML and one stylesheet.

| Path | What |
| --- | --- |
| `index.html` | Landing page (English) |
| `nl/index.html` | Landing page (Dutch) |
| `privacy/index.html` | Privacy policy — the URL for the Play Console |
| `app-ads.txt` | AdMob seller declaration |
| `assets/` | Icon, feature graphic, screenshots (JPEG, 540×960), `site.css` |

## Publishing

Repository *Settings → Pages → Build and deployment*: source **Deploy from a branch**, branch `main`, folder `/ (root)`.

* Privacy policy URL: `https://<user>.github.io/<repo>/privacy/`
* `app-ads.txt` only counts at the **root of a domain**. AdMob looks for it at the domain of the developer website in
  the Play listing, so either name this repository `<user>.github.io` or give the site its own domain (add a `CNAME`
  file and a DNS record), and use that address as the website in the Play Console.

## Notes

The Google Play badges are loaded from Google (official badge images); the links point to
`https://play.google.com/store/apps/details?id=nl.bluecard.app` and work once the app is public.

## Preview locally

```bash
python3 -m http.server 8765
```
