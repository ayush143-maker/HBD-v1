# HBD-v1

A personalised birthday microsite for Anya, with animated typography and a sequence of visual sections. The experience is contained in the top-level `index.html`; preserve the paths to referenced images when updating assets.

## Preview locally

No package installation is required. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit http://localhost:8000. After changing the greeting or media, review the page at phone and desktop viewport sizes and check that referenced images appear. If an image is missing, confirm that its path in `index.html` matches its location. No deployment configuration is documented; serve the page and its images as static files with their relative paths intact.