# V10 — pixel-perfect Figma email

This implementation uses the uploaded Figma PNG export (`1200 × 8678 px`) as its visual source. It is cut into eight lossless PNG slices and displayed at `600 px` wide, so the delivered visual matches the Figma export 1:1.

## Why this implementation

- no reconstructed fonts, spacing, or product compositions;
- no GIF, CSS animation, or unsupported webfont dependency;
- stable in Gmail, Outlook, Mail.ru, Yandex Mail and Apple Mail because it relies on standard linked images in a table container;
- each semantic email section is linked to the appropriate category or blog destination.

## Production handoff

1. Upload files in `assets/` to the ESP/CDN; do not use GitHub RAW in a final campaign.
2. Replace the category and blog URLs with final deeplinks / UTM labels.
3. If every product card needs its own URL, export the Figma frame as additional card-level slices; HTML email does not reliably support image maps across clients.
4. Add the ESP-required legal footer/unsubscribe module if it is not injected automatically.

The total asset payload is approximately 4.3 MB. It is intentionally close to the original Figma PNG to preserve small text and the exact layout. If delivery-weight limits require it, optimize each slice after visual approval.
