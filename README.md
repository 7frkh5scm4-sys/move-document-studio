# Move Document Studio

Resize, reflow, and crop PDF, DOCX, and RTF files for a 7.3-inch e-ink reader (324 × 576 pt pages). Everything runs on your device. Nothing is uploaded.

## Version 4.0

Two modes:

- **Continuous reading (PDF artwork):** keeps the original page artwork, trims margins, and carries pages into unused space. Output is PDF.
- **Reformat document (text):** rebuilds PDF, DOCX, or RTF text. Choose the output format:
  - **PDF:** fixed pages at a custom text size.
  - **EPUB:** reflowable, so font, size, margins, and spacing are set on the reader. Keeps all characters and supported RTF PNG/JPEG pictures.

Also:

- Works offline. Libraries (pdf.js 3.11.174, pdf-lib 1.17.1, mammoth 1.8.0, JSZip 3.10.1) are in `vendor/`.
- Installable from a browser with Add to Home Screen.
- Remembers your last mode and output format on each device.
- Output names: `-move-continuous-<size>.pdf`, `-move-read.pdf`, `-move.epub`.

## Hosting with GitHub Pages

Settings > Pages > Build and deployment > Deploy from a branch > `main` / root. The site appears at `https://<username>.github.io/move-document-studio/`.

## Updating

When you change any file, bump the `CACHE` name at the top of `sw.js` (for example `mds-3.6.1`). Otherwise installed copies keep serving the old files.

## Files

- `index.html` – the app
- `vendor/` – bundled libraries
- `icons/`, `manifest.webmanifest` – home-screen install
- `sw.js` – offline cache
