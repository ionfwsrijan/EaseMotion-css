# Animal Card Flip

3D flip card that reveals animal information on hover.

## Usage

```html
<link rel="stylesheet" href="style.css" />

<div class="flip-card">
  <div class="flip-card-inner">
    <div class="flip-card-front">
      <span class="animal">🐶</span>
      <span class="label">Dog</span>
    </div>
    <div class="flip-card-back">
      <h3>Dog</h3>
      <p>Description text here.</p>
    </div>
  </div>
</div>
```

## CSS Custom Properties

| Property | Default | Description |
|---|---|---|
| `--card-front` | `#2d2d44` | Front face background color |
| `--card-back` | `#4ecdc4` | Back face background color |
| `--flip-duration` | `0.6s` | Flip animation duration |

## Behavior

Cards flip on hover/focus using CSS 3D transforms (`rotateY`). The back face uses `backface-visibility: hidden` and is pre-rotated 180deg.
