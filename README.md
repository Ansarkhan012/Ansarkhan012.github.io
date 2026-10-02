# Ansar Games website

Static site (plain HTML/CSS) served by GitHub Pages at **https://ansarkhan012.github.io/**.

| Page | URL |
|---|---|
| Ansar Games home | https://ansarkhan012.github.io/ |
| Zen Sort app page | https://ansarkhan012.github.io/zen-sort/ |
| Zen Sort privacy policy | https://ansarkhan012.github.io/zen-sort/privacy-policy.html |

## Structure

```
index.html                    Ansar Games home (game cards)
zen-sort/index.html           Zen Sort app page (support + privacy links)
zen-sort/privacy-policy.html  Zen Sort privacy policy (effective October 2, 2026)
assets/style.css              Shared calm pastel style (light + dark mode)
assets/*.png                  Icons generated from the app's assets/icon/app_icon.png
.nojekyll                     Serve files as-is (no Jekyll processing)
```

No build step, no tracking scripts, and no external fonts: the site uses the system font stack, so visiting it doesn't send data to third parties.

## GitHub Pages

Settings → Pages → **Build and deployment: Deploy from a branch** → Branch **main**, folder **/ (root)**.

## app-ads.txt

`app-ads.txt` is at the root of this site, as AdMob requires:
https://ansarkhan012.github.io/app-ads.txt

```
google.com, pub-6939327867611226, DIRECT, f08c47fec0942fa0
```

Keep `https://ansarkhan012.github.io/` in the **Website** field of the Google Play store listing: AdMob looks for `app-ads.txt` on that domain. Verification in AdMob (Apps → View all apps → app-ads.txt) can take up to 24 hours.

## Updating the privacy policy

When the app adds or removes a service (SDK) or starts collecting new data, update `zen-sort/privacy-policy.html` and change the effective date.
