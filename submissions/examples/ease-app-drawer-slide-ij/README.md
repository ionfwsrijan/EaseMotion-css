# App Drawer Slide

A bottom drawer component that slides up with an overlay backdrop.

## Usage

```html
<link rel="stylesheet" href="style.css" />

<button class="drawer-toggle">Open Drawer</button>

<div class="drawer-overlay"></div>

<div class="drawer">
  <div class="drawer-handle"></div>
  <div class="drawer-icons">
    <div class="drawer-icon">⚙️</div>
  </div>
</div>

<script>
  const toggle = document.querySelector('.drawer-toggle');
  const drawer = document.querySelector('.drawer');
  const overlay = document.querySelector('.drawer-overlay');

  toggle.addEventListener('click', () => {
    drawer.classList.add('open');
    overlay.classList.add('visible');
  });

  overlay.addEventListener('click', () => {
    drawer.classList.remove('open');
    overlay.classList.remove('visible');
  });
</script>
```

## CSS Custom Properties

| Property | Default | Description |
|---|---|---|
| `--drawer-bg` | `#2d2d44` | Drawer background color |
| `--icon-color` | `#4ecdc4` | Icon accent color |
| `--slide-duration` | `0.3s` | Slide animation duration |

## Behavior

Toggle button opens the drawer (slides up from bottom). Overlay click closes it. The drawer uses `transform: translateY(100%)` / `translateY(0)` for smooth sliding.
