# GitAfterIt — marketing site

Static marketing landing page for **[gitafterit.app](https://gitafterit.app)**.

GitAfterIt is a native iOS app: a home for your GitHub repositories, pull
requests, terminals, and Copilot coding agents.

## Structure

No build step — plain HTML/CSS, deploy the folder as-is.

```
index.html          # landing page
privacy.html        # privacy policy (required for App Store)
assets/
  styles.css        # all styles
  icon.png          # app icon (1024×1024)
  favicon.png
  apple-touch-icon.png
  screenshots/      # iPhone screenshots (1206×2622)
```

## Local preview

```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## Deploy (Cloudflare Pages)

1. Create a Pages project connected to this repo.
2. **Framework preset:** None. **Build command:** _(empty)_. **Output directory:** `/`.
3. Add the custom domain `gitafterit.app` in the Pages project and point DNS at Cloudflare.

## To finish before launch

- [ ] Replace the **"Coming soon"** buttons (`data-cta="testflight"`) with your
      TestFlight public link, e.g. `https://testflight.apple.com/join/XXXXXXXX`.
- [ ] Update the contact email in `privacy.html`.
- [ ] Swap in an App Store badge/link once the app is live.
