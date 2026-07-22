# V12 — refined Figma HTML

This version keeps the Figma-based live HTML approach but corrects the component hierarchy requested in review:

- product card radii and CTA radii are deliberately distinct from cart controls;
- the uploaded Figma `-15%.svg` is stored with the implementation for the source badge;
- pale blue `#F2FAFC` surfaces are retained under the appropriate category modules;
- all major semantic modules use a 50 px vertical gap;
- button labels use sentence case and Ubuntu regular weight;
- CTA hover is `#5E8C17`;
- article “Читать” actions use white background / blue text on hover;
- regular CTA buttons do not have underlines.

Production note: replace GitHub RAW asset paths with ESP/CDN URLs and use a PNG rendering of `discount-15.svg` for Outlook compatibility.
