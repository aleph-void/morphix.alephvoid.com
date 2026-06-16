# morphix.alephvoid.com

Marketing site for **Morphix** — a polyphonic morphing wavetable synthesizer plugin
(AUv3 / VST3 / Standalone), a from-scratch reconstruction of the lost 2005 *FSR Morphite*,
themed in the [Aleph Void](https://alephvoid.com) visual language.

A static site (plain HTML/CSS/JS, no build step) intended for GitHub Pages at
`https://morphix.alephvoid.com`.

## Pages

| File           | Purpose                                            |
|----------------|----------------------------------------------------|
| `index.html`   | Landing page — features, signal path, screenshots, specs, download, FAQ |
| `support.html` | Support channels, pre-filing checklist, troubleshooting |
| `privacy.html` | Privacy policy (Morphix collects nothing, makes no network requests) |

## Structure

```
.
├── index.html
├── support.html
├── privacy.html
├── styles.css                 Aleph Void dark theme (shared by all pages)
├── main.js                    Mobile menu, nav shadow, screenshot lightbox
├── CNAME                      morphix.alephvoid.com
├── .gitignore
├── .github/
│   └── ISSUE_TEMPLATE/        Bug report / feature request templates + config
└── assets/
    ├── img/
    │   ├── app-icon.png        Morphix plugin icon (256)
    │   ├── app-icon-1024.png   Morphix plugin icon (1024)
    │   ├── logo.svg            Morphix square icon (SVG)
    │   └── wordmark.svg        Morphix horizontal wordmark
    └── screenshots/
        ├── macos/             ← drop macOS screenshots here
        └── ios/               ← drop iOS / iPadOS screenshots here
```

## Adding screenshots

Drop image files into `assets/screenshots/macos/` or `assets/screenshots/ios/`, then add a
`<figure class="shot">` entry to the matching grid in `index.html` (`#shots-macos` /
`#shots-ios`). Each folder's `README.md` has copy-paste markup and tips. Clicking a
screenshot opens it in a lightbox automatically.

## Reporting bugs

Found a bug or have a feature request? Please open an issue on the tracker:

**https://github.com/aleph-void/morphix.alephvoid.com/issues**

Issue templates for bug reports and feature requests live in
[`.github/ISSUE_TEMPLATE/`](.github/ISSUE_TEMPLATE/). For a bug, include your OS and
version, the Morphix version, the plugin format (AUv3 / VST3 / Standalone), and your
host / DAW. You can also email <support@alephvoid.com> if you'd rather not file publicly.

## Local preview

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Branding

Aleph Void dark palette — void background `#0a0a0f`, violet accent `#6d28d9` / `#8b5cf6`,
Inter + JetBrains Mono. Brand assets are sourced from the Morphix plugin repo
(`Morphix/assets/brand` and `Morphix/assets/icons`).

---

© 2026 Aleph Void LLC. Morphix is an independent reconstruction; the original *FSR Morphite*
is referenced only as the historical source of the recovered design and presets.
