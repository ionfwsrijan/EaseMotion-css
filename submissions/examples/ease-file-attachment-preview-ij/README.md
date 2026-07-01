# File Attachment Preview

## What does this do?

Creates animated file preview cards that slide in when files are uploaded. Each card displays the filename, file size, and a hover-reveal remove button.

## How is it used?

Add the `fap-card` class to your file preview elements and apply the `fap-visible` class to trigger the slide-in animation:

```html
<div class="fap-card fap-visible">
  <div class="fap-info">
    <span class="fap-name">document.pdf</span>
    <span class="fap-size">2.4 MB</span>
  </div>
  <button class="fap-remove">Remove</button>
</div>
```

Configure parameters with custom CSS variables:
- `--fap-radius`: Border radius of the card (defaults to `0.75rem`).
- `--fap-bg`: Card background color (defaults to `var(--ease-color-surface)`).
- `--fap-border`: Card border color (defaults to `var(--ease-color-neutral-200)`).
- `--fap-remove-bg`: Background color of the remove button (defaults to `#ef4444`).
- `--fap-remove-color`: Text color of the remove button (defaults to `#fff`).
- `--fap-transition`: Transition timing for card animations (defaults to `0.35s cubic-bezier(0.16, 1, 0.3, 1)`).

## Why is this useful?

File upload previews are a common UI pattern in dashboards, messaging apps, and document management systems. This component provides a polished, accessible slide-in animation that draws attention to newly added files without being distracting. The hover-reveal remove button keeps the interface clean, and reduced-motion support ensures a smooth experience for all users.
