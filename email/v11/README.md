# V11 — Figma structure implementation

V11 is the live-HTML implementation based on `figma-structure.json`, exported from the Figma frame rather than inferred from a screenshot.

## Locked Figma values

- Frame: 600 × 4339 px
- Blue: #0073AE
- Green: #80BA27
- Light surface: #F2FAFC
- Text: #1D3842 / #657D82
- Typography: Ubuntu (400 / 500 / 700) with `Arial, Helvetica, sans-serif` fallback
- Header content and full product structure follow the 146-element export.

## Implementation details

- all ten products retain separate visual cards, price, discount treatment and cart control;
- top header, promo tickers, category sections, two editorial blocks and footer are table based;
- no GIF or CSS animation;
- `figma-structure.json` is committed alongside the code to make design-to-code comparison possible.

Before sending, move images to the ESP/CDN, supply final item/blog URLs and replace `{{unsubscribe_url}}`.
