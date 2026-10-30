# HBD-v1

HBD-v1 is a personalized birthday tribute for Anya and Arjun, presented as a sequence of animated visual sections. The page includes an interactive gift, candle-lit cake, compliment balloons, photos, and a celebratory finale. Its top-level `index.html` is the entry point; review the names and personal details before reusing or publishing it.

## Preview locally

No package installation is required. Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). For static hosting, publish the page and its referenced images with their relative paths intact.

## Birthday interactions

Tap the gift to open or close the friendship voucher; its expanded/hidden accessibility state updates with the interaction. The cake takes two taps: the first lights the candles and the next blows them out and reveals the wish. A separate button can relight the cake after the wish appears.

Five compliment balloons can be popped one at a time. Popping all five reveals a completion message, and a button restores the balloons so visitors can pop them again. The fixed confetti button launches confetti on demand; another confetti burst plays when the finale first enters view. Taps in selected sections also create sparkles. Gift, cake, and balloon state is held by the page and does not persist between reloads.

## Photos, motion, and editing

The four photo paths are `images/photo-01.jpg` through `images/photo-04.jpg`. Failed image loads are replaced with inline illustrated SVGs, and some photos load lazily. Keep the image files at those paths or update the references in `index.html` when moving or replacing them.

Sections reveal as visitors scroll, and selected photos use parallax. CSS responds to reduced-motion preferences by disabling or shortening animations and transitions. Fraunces, Instrument Serif, and Plus Jakarta Sans are loaded from Google Fonts, so those typefaces require network access; retain readable fallback styles if fonts cannot load.

Edit the page’s copy, styles, interactions, and title in `index.html`. The source makes no application API calls and uses no local or session storage. Its interaction state is page-only. Review the names, message, and photos before sharing; no birthday content or interaction state is sent to an application service by the page.