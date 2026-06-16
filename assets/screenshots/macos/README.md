# macOS screenshots

Drop macOS screenshots of Morphix here (PNG or JPG).

These show the plugin running in a DAW (AUv3 / VST3) or as the Standalone app on macOS.

## How to wire them into the site

1. Save your image files into this folder, e.g. `osc.png`, `filter.png`, `presets.png`.
2. Open `index.html` and find the `#shots-macos` grid in the Screenshots section.
3. Remove the `.shot-empty` placeholder and add one `<figure>` per image:

   ```html
   <figure class="shot">
     <img src="assets/screenshots/macos/osc.png" alt="Morphix oscillator page on macOS" loading="lazy" />
     <figcaption>Oscillator &amp; morph</figcaption>
   </figure>
   ```

Clicking a screenshot opens it in the lightbox automatically (handled by `main.js`).

## Suggested shots

- Oscillator / morph page
- Filter & envelopes
- LFO & modulation
- Flanger / FX
- Preset browser
- Full plugin window in a host (Logic, Ableton Live, etc.)

Recommended: 3:2 aspect ratio for a tidy grid (the thumbnails are cropped to 3:2).
