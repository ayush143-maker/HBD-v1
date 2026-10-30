# HBD-v1

A personalised birthday microsite for Anya, with animated typography and a sequence of visual sections. The experience is contained in the top-level `index.html`; preserve the paths to referenced images when updating assets.

## Preview locally

No package installation is required. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit http://localhost:8000. No deployment configuration is documented; serve the page and its images as static files with their relative paths intact.

## Personalizing the page

Edit the greeting and visible section content in `index.html`. The page title is “Happy Birthday, Anya ✦”; update it too if you are personalizing the page for someone else. The document uses Fraunces, Instrument Serif, and Plus Jakarta Sans from Google Fonts, so if you change typefaces, keep the font link and the page's corresponding font styling in sync.

Before moving or replacing an image, check its existing reference in `index.html`. Keep the same relative location, or update the reference to the new location.

## Manual review checklist

Use these actions to review the page; they are not verified results.

- Open the known entry page, `index.html`, in a browser, or visit `http://localhost:8000` after starting the local server above.
- Read the greeting and scroll through the sequence of visual sections. Observe the animated typography after any related changes.
- Check each referenced image path in `index.html` against the image's actual location, then view the page and confirm the images are available.
- Inspect the page at a narrow phone-sized viewport and a wide desktop-sized viewport. Check text wrapping, section layout, and image presentation.
- If you changed typefaces, check that the Google Fonts link and the corresponding styling in `index.html` stay aligned.
