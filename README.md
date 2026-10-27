# Mr. Smith's Aero Labs

Interactive aerospace labs for class, published with GitHub Pages. Each lab is one folder of self-contained files so it can run on school Chromebooks without outside downloads.

## Folder-per-lab layout

The site root is the home page. Every lab is a folder next to it, and that folder name is the URL path.

```
index.html            home page
.nojekyll             tell GitHub Pages to skip Jekyll
wind-tunnel/
  index.html          Wind Tunnel Lab
```

To add a lab, add a new folder with its own `index.html`, then add a link to that folder on the home page.

## Public URLs

- Home: https://gatoraero.github.io/aero-labs/
- Wind Tunnel Lab: https://gatoraero.github.io/aero-labs/wind-tunnel/

## Canvas

A lab can be embedded in Canvas with an iframe:

```html
<iframe src="https://gatoraero.github.io/aero-labs/wind-tunnel/" title="Wind Tunnel Lab" width="100%" height="800" style="border:0" allow="fullscreen"></iframe>
```

## Publishing

Pushes to `main` deploy the repository root through `.github/workflows/pages.yml`. Pages must use the GitHub Actions source (build type `workflow`).
