# Rekludo site (rekludo.com)

One static page for the Rekludo party game: plain HTML and CSS, no framework, no build step, no cookies and no outside requests (the font is hosted here).

## Preview
Open `index.html` in a browser.

## Files
| File | What |
| --- | --- |
| `index.html`, `style.css` | The page and its styles |
| `img/` | Screenshots (compressed), icons, social card (`og-image.jpg`, 1200x630) |
| `fonts/` | Big Shoulders (SIL Open Font License, `OFL.txt` stays with it) |
| `404.html`, `robots.txt`, `sitemap.xml` | Housekeeping |

## Not live yet
This repo is not published. To go live:
1. Repo Settings, Pages, deploy from branch `main`, folder `/ (root)`.
2. Add a `CNAME` file containing `rekludo.com`, then point the domain's DNS at GitHub Pages (A records for the apex, a CNAME for `www`), and tick "Enforce HTTPS".
3. Link manic.club's "First up: RekludØ" line to rekludo.com.

## Launch-day swaps
- Replace both **Coming soon** buttons (hero and closing call) with the App Store badge linking to `https://apps.apple.com/app/id6835205482`.
- Uncomment the **Smart App Banner** meta tag in `index.html` (`app-id=6835205482`).
- Replace the screenshots in `img/` if the game's look has changed.
- Put the AdMob `app-ads.txt` line in a file called `app-ads.txt` at the root (or on manic.club, whichever domain the App Store listing's marketing URL uses).
- Privacy and Support live on manic.club: `https://manic.club/privacy/rekludo/` and `https://manic.club/support/`.
