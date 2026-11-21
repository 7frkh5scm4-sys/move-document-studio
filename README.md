# Move Document Studio

Resize, reflow, and crop PDF, DOCX, and RTF files for a 7.3-inch e-ink reader (324 × 576 pt pages). Everything runs on your device. Nothing is uploaded.

## Version 3.6

- Works offline. The libraries (pdf.js 3.11.174, pdf-lib 1.17.1, mammoth 1.8.0, JSZip 3.10.1) are in `vendor/` instead of loading from a CDN.
- Installable. Open the hosted page on a phone or tablet and choose Add to Home Screen.
- Phone layout with safe-area padding.
- Conversion logic is unchanged from 3.5.

## Hosting with GitHub Pages

Settings > Pages > Build and deployment > Deploy from a branch > `main` / root. The site appears at `https://<username>.github.io/move-document-studio/`.

## Updating

When you change any file, bump the `CACHE` name at the top of `sw.js` (for example `mds-3.6.1`). Otherwise installed copies keep serving the old files.

## Files

- `index.html` – the app
- `vendor/` – bundled libraries
- `icons/`, `manifest.webmanifest` – home-screen install
- `sw.js` – offline cache
