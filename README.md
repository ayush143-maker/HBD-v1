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

## Configuration and data handling

This repository is a static page centered on `index.html`; no environment template or backend configuration is listed. Do not put credentials or other private values in tracked files. Values embedded in a static page are delivered to visitors and cannot be kept secret. The greeting and referenced images are page content; review names, personal details, and media before sharing or publishing the page. Google Fonts are loaded from an external service, so browsers may make requests to Google to retrieve the linked fonts.

## Browser and layout review checklist

This is a checklist for future review, not a report of completed compatibility testing or verified results.

- Open `index.html` in current versions of browsers relevant to the page's intended audience. Also load it through the local server above to review relative paths in a served-page context.
- Read the greeting and scroll through the visual sections. Observe the animated typography after related edits.
- Inspect the browser console during page load and while scrolling or viewing animations. Investigate errors that may affect content or presentation.
- Inspect the Network panel for failed requests. Check every local image reference in `index.html` against the file at that relative path and confirm images display. Check requests for Fraunces, Instrument Serif, and Plus Jakarta Sans from Google Fonts; confirm remote font loading is intentional and review how the page looks if those requests fail.
- Inspect the page at a narrow phone-sized viewport and a wide desktop-sized viewport. Check text wrapping, section layout, and image presentation for clipping or overflow.
- Review image dimensions and file sizes for their use. Before removing a file, check that no page or style still references it; update paths when moving assets.

## Accessibility review checklist

Use these as future review steps; they are not verified results.

- Navigate through the page using only a keyboard. Check that any links or controls encountered can receive focus and be activated without a pointer.
- Check that keyboard focus remains visible and is not lost against decorative backgrounds.
- Review links and controls for clear, meaningful names. Check that the greeting and section text remain understandable without relying on animated typography or visual styling alone.
- Check text contrast across the page, including the greeting and text placed over decorative backgrounds.
- For each referenced image, check whether it conveys information that needs a text alternative; avoid redundant descriptions for purely decorative images.
- Check animated typography and other motion with reduced motion requested. Consider reducing or stopping nonessential animation.