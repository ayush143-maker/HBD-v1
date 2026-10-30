# HBD-v1

HBD-v1 is a personalised birthday microsite for Anya, with animated typography and a sequence of visual sections. The top-level `index.html` is the page entry point and has the title “Happy Birthday, Anya ✦”.

## Preview locally

No package installation is required. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). No build or deployment configuration is documented; serve the page and its referenced images as static files with their relative paths intact.

## Personalize the page

Edit the greeting and visible section content in `index.html`. If adapting the page for someone else, update the document title as well as the visible message. The page requests Fraunces, Instrument Serif, and Plus Jakarta Sans from Google Fonts; these requests require network access. If changing typefaces, keep the font links and corresponding page styling in sync.

Before moving or replacing an image, check its existing reference in `index.html`. Keep the image at its referenced relative path or update the reference to match its new location. Review names, personal details, and media before sharing or publishing this personalized page.

## Repository map

- `index.html` — page entry point, content, styling, and image references.

After editing, preview the greeting, visual sections, animated typography, and images in a browser at narrow and wide viewport sizes. Check for clipping or overflow. No separate asset directory or deployment setup is identified here.