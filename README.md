# hydtek.ca

Static site for Hydtek, served by GitHub Pages at https://hydtek.ca. Plain HTML/CSS, no build step, no trackers.

- `/` — Hydtek landing page
- `/tvplayer/privacy/`, `/tvplayer/terms/`, `/tvplayer/support/` — TekTV policies and support (linked from the app's Settings and App Store Connect)
- `/app-ads.txt` — AdMob authorised sellers (must stay at the domain root)
- `CNAME` — custom domain for GitHub Pages

The contact email appears on several pages; to change it everywhere:

    for f in index.html tvplayer/*/index.html; do sed -i '' 's/support@hydtek.ca/NEW@EXAMPLE.COM/g' "$f"; done

