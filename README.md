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

Use these actions to review the page; they are not verified results or measured performance.

- Open `index.html` in a browser, or visit `http://localhost:8000` after starting the local server above.
- Read the greeting and scroll through the sequence of visual sections. Observe the animated typography after any related changes.
- Check every local image, audio, and font reference in `index.html` against a file at the referenced path. Confirm the images display after loading the page.
- Review image and audio file sizes and dimensions for their use on the page. Avoid oversized media, and remove files only after checking that no page or style still references them.
- The page links to Fraunces, Instrument Serif, and Plus Jakarta Sans through Google Fonts. Confirm that the external font dependency is intentional and each linked family is used; if typography changes, update the link and matching styles together. Review any external script references for the same purpose before retaining or adding them.
- Inspect the page at a narrow phone-sized viewport and a wide desktop-sized viewport. Check text wrapping, section layout, and image presentation.

## Accessibility review checklist

Use these as future review steps; they are not verified results.

- Navigate through the page using only a keyboard. Check that any links or controls encountered can receive focus and be activated without a pointer.
- Check that keyboard focus remains visible as you move through the page and is not lost against decorative backgrounds.
- Review any links or controls for clear, meaningful names. Check that the greeting and section text remain understandable without relying on animated typography or visual styling alone.
- Check text contrast across the page, including the greeting and text placed over decorative backgrounds.
- For each referenced image, check whether it conveys information that needs a text alternative; avoid redundant descriptions for purely decorative images.
- Check animated typography and other motion with reduced motion requested. Consider reducing or stopping nonessential animation.