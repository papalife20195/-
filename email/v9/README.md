# HTML email from Figma export

This version is rebuilt from the supplied Figma export, not from an approximate visual reference.

## Exact values obtained from the export

- container: 600 px;
- primary blue: `#0073AE`;
- heading / button green: `#80BA27`;
- light section surface: `#F2FAFC`;
- typeface specified by the designer: Ubuntu, with fallbacks `Arial, Helvetica, sans-serif`.

## Included source content

All five product categories, 10 named product cards and prices, both discount mechanics, both blog teasers, the hero, final category CTA and footer are included.

The supplied Figma assets are embedded in the repository as optimized JPG/PNG files for email use. SVG originals remain in the user-provided ZIP on `main`; production email uses raster images for client compatibility.

Before production, move the GitHub RAW image URLs to CDN/ESP storage, fill final product/blog URLs and replace `{{unsubscribe_url}}` with the ESP variable.

## Figma fidelity update

V9 now includes the Figma-style green `–15%` overlay badge on every discounted product image and the original exported green cart button next to every price. Light category surfaces and rounded product modules are preserved in the HTML layout.
