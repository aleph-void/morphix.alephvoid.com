# iOS / iPadOS screenshots

Drop iPhone and iPad screenshots of Morphix here (PNG or JPG).

These show the AUv3 running in a host (GarageBand, AUM, Cubasis) or the Standalone app on iOS / iPadOS.

## How to wire them into the site

1. Save your image files into this folder, e.g. `ipad-osc.png`, `iphone-presets.png`.
2. Open `index.html` and find the `#shots-ios` grid in the Screenshots section.
3. Remove the `.shot-empty` placeholder and add one `<figure>` per image:

   ```html
   <figure class="shot">
     <img src="assets/screenshots/ios/ipad-osc.png" alt="Morphix oscillator page on iPad" loading="lazy" />
     <figcaption>Oscillator &amp; morph (iPad)</figcaption>
   </figure>
   ```

Clicking a screenshot opens it in the lightbox automatically (handled by `main.js`).

## Suggested shots

- AUv3 loaded in GarageBand / AUM / Cubasis
- Standalone app, full screen on iPad
- Preset browser on iPhone
- Filter & envelopes
- LFO & modulation

Recommended: 3:2 aspect ratio for a tidy grid (the thumbnails are cropped to 3:2).
Tall phone screenshots still work — they're cropped to fit the thumbnail and shown in full in the lightbox.
