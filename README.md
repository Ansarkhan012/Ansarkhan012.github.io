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

## TODO: app-ads.txt (not created yet)

AdMob needs an `app-ads.txt` file at the **root** of this site:
`https://ansarkhan012.github.io/app-ads.txt`

Once you have your AdMob publisher ID (`pub-XXXXXXXXXXXXXXXX`, shown in AdMob → Settings → Account information), create `app-ads.txt` in the root of this repo containing exactly the line AdMob shows you, for example:

```
google.com, pub-XXXXXXXXXXXXXXXX, DIRECT, f08c47fec0942fa0
```

Also put `https://ansarkhan012.github.io/` in the **Website** field of the Google Play store listing, because AdMob looks for `app-ads.txt` on that domain. Verification in AdMob can take up to 24 hours.

## Updating the privacy policy

When the app adds or removes a service (SDK) or starts collecting new data, update `zen-sort/privacy-policy.html` and change the effective date.
