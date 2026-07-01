# Color Swatch Picker

## What does this do?

It creates an interactive grid of circular color swatches that users can click to select a color. A selected swatch displays a ring (`box-shadow`) and an animated checkmark overlay (`::after` pseudo-element) for clear visual feedback.

## How is it used?

Add the `csp-swatch` class to any element and set the `--csp-color` custom property. Toggle the `csp-selected` class to show the selection ring and checkmark.

```html
<button class="csp-swatch" style="--csp-color: #3b82f6"></button>
<button class="csp-swatch csp-selected" style="--csp-color: #ef4444"></button>
```

You can customize the component with these CSS variables:

- `--csp-swatch-size`: Diameter of each swatch circle (defaults to `2.5rem`).
- `--csp-ring-color`: Color of the selection ring (defaults to `#6c63ff`).
- `--csp-ring-width`: Thickness of the selection ring (defaults to `3px`).
- `--csp-check-color`: Color of the checkmark icon (defaults to `#ffffff`).
- `--csp-transition-duration`: Speed of the scale and opacity transitions (defaults to `0.2s`).

## Why is this useful?

A visual color picker is a common UI pattern in design tools, theme editors, and settings panels. This component keeps the selection feedback smooth and compositor-friendly by animating only `transform` and `opacity`, ensuring 60&nbsp;fps interactions on most devices. It degrades gracefully when users prefer reduced motion.
