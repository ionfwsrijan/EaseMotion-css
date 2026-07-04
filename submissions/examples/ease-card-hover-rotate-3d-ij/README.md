# Card Hover Rotate 3D

A CSS-only 3D card that rotates in perspective space on hover, with a front and back face using `backface-visibility`.

## HTML Structure

```html
<div class="ease-card-hover-rotate-3d">
  <div class="card-scene">
    <div class="card-3d">
      <div class="card-face card-front">...</div>
      <div class="card-face card-back">...</div>
    </div>
  </div>
</div>
```

Hover over `.card-3d` to trigger the rotation. The front face is shown by default; the back face is revealed on hover.

## CSS Variables

| Variable | Default | Description |
|---|---|---|
| `--card-bg` | `linear-gradient(135deg, #667eea, #764ba2)` | Background of the front card face |
| `--rotate-x` | `15deg` | Rotation angle on the X axis on hover |
| `--rotate-y` | `15deg` | Rotation angle on the Y axis on hover |
| `--perspective` | `800px` | Perspective value for the 3D scene |
| `--transition-speed` | `0.4s` | Duration of the rotation transition |
