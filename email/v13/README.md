# V13 — corrected email components

This revision deliberately replaces the parts that were not actually email-safe in V12:

- `discount-15-email.png` is a visible, raster, static badge; no SVG or GIF is used in the email itself.
- Each supplied square product visual has a transparent raster rounded-corner mask (14 px display radius) instead of relying on `border-radius` support.
- Global anchors have no underline. Footer may use separate non-button styling only if required.
- Cart uses its own rounded image button. A `:hover` state swaps to `#5E8C17`; non-supporting email clients retain the normal green state.
- Normal CTA hover is `#5E8C17`; `Читать` uses a white hover state with blue text.
- Major semantic modules retain 50 px spacing.
