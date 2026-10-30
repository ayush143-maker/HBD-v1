# HBD-v1

A personalised birthday microsite for Anya, with animated typography and a sequence of visual sections. The experience is contained in the top-level `index.html`; preserve the paths to referenced images when updating assets.

## Preview locally

No package installation is required. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit http://localhost:8000. After changing the greeting or media, review the page at phone and desktop viewport sizes and check that referenced images appear. If an image is missing, confirm that its path in `index.html` matches its location. No deployment configuration is documented; serve the page and its images as static files with their relative paths intact.

## Personalizing the page

Edit the greeting and visible section content in `index.html`. The page title is “Happy Birthday, Anya ✦”; update it too if you are personalizing the page for someone else. The document uses Fraunces, Instrument Serif, and Plus Jakarta Sans from Google Fonts, so if you change typefaces, keep the font link and the page's corresponding font styling in sync.

Before moving or replacing an image, check its existing reference in `index.html`. Keep the same relative location, or update the reference to the new location, then preview the page at phone and desktop sizes to check both the text and media.