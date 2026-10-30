# HBD-v1

A personalised birthday microsite for Anya, with animated typography and a sequence of visual sections. The experience is contained in the top-level `index.html`; preserve the paths to referenced images when updating assets.

## Preview locally

No package installation is required. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit http://localhost:8000. No deployment configuration is documented; serve the page and its images as static files with their relative paths intact.

## Personalizing the page

Edit the greeting and visible section content in `index.html`. The page title is “Happy Birthday, Anya ✦”; update it too if personalizing the page for someone else. The page requests Fraunces, Instrument Serif, and Plus Jakarta Sans from Google Fonts. If you change typefaces, keep the font link and corresponding page styling in sync.

Before moving or replacing an image, check its existing reference in `index.html`. Keep its relative location or update the reference to match the new location. The Google Fonts requests depend on network access to that service.

## Deployment-readiness checklist

This repository documents a static page, with its experience in the top-level `index.html`. No build or deployment configuration is specified. Before publishing:

- [ ] Use the repository root as the page's document root, so the top-level `index.html` is served as the page.
- [ ] Include the images referenced by `index.html` at paths that preserve those references, or update the references to match any changed locations. Check the actual references before moving or replacing images.
- [ ] The page requests Fraunces, Instrument Serif, and Plus Jakarta Sans from Google Fonts. These requests depend on network access to that service; check that the page remains legible if the requests are unavailable.
- [ ] No environment-variable template is listed, so no environment configuration is indicated by this repository.
- [ ] Review the personalized greeting, name, personal details, and media before sharing or publishing.
- [ ] After publishing, open the resulting page in a browser. Review the greeting, visual sections, animated typography, and image presentation at narrow phone-sized and wide desktop-sized viewports, checking for clipping or overflow.
- [ ] These are recommendations for the final preview, not claims that publishing or browser checks have already occurred.

## Contributor handoff

Keep changes scoped to the relevant content, styling, or image references in `index.html`. Preserve the filename and existing relative paths unless a change requires updating them; when moving or replacing an image, update its reference. In the handoff, summarize what changed and identify the affected page area or file. Review names, personal details, and media before sharing or publishing this personalized page.

Before publishing, manually review the greeting and visual sections in a browser. Check animated typography and image presentation at a narrow phone-sized viewport and a wide desktop-sized viewport, looking for clipping or overflow. This is a review checklist, not a report of completed browser checks or verified results.
