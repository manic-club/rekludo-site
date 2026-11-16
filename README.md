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

## Hosting
GitHub Pages, from branch `main`, folder `/ (root)`. The custom domain is `rekludo.com` (the `CNAME` file; do not delete it).

DNS at the registrar (remove any parking or forwarding records first):
- `A` records for `rekludo.com`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- `AAAA` records for `rekludo.com`: `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`
- `CNAME` for `www`: `manic-club.github.io`

When GitHub has checked the DNS, tick "Enforce HTTPS" in the repo's Pages settings. Optional but recommended: verify the domain for the manic-club organisation (org Settings, Pages, Add a domain, add the TXT record GitHub shows) so nobody else can claim it.

## Launch-day swaps
- Replace both **Coming soon** buttons (hero and closing call) with the App Store badge linking to `https://apps.apple.com/app/id6835205482`.
- Uncomment the **Smart App Banner** meta tag in `index.html` (`app-id=6835205482`).
- Replace the screenshots in `img/` if the game's look has changed.
- Put the AdMob `app-ads.txt` line in a file called `app-ads.txt` at the root (or on manic.club, whichever domain the App Store listing's marketing URL uses).
- Privacy and Support live on manic.club: `https://manic.club/privacy/rekludo/` and `https://manic.club/support/`.
