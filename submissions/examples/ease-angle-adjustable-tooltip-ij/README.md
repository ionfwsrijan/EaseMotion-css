# Angle Adjustable Tooltip

A tooltip component with an adjustable arrow angle and pop-in animation.

## Usage

```html
<link rel="stylesheet" href="style.css" />

<div class="tooltip-wrapper">
  <button class="trigger">Hover me</button>
  <div class="tooltip" role="tooltip">
    <span class="tooltip-text">Tooltip content</span>
    <div class="tooltip-arrow"></div>
  </div>
</div>
```

## CSS Custom Properties

| Property | Default | Description |
|---|---|---|
| `--tooltip-bg` | `#333` | Tooltip background color |
| `--arrow-color` | `#4ecdc4` | Arrow color |
| `--pop-duration` | `0.2s` | Pop-in animation duration |
| `--arrow-angle` | `180deg` | Arrow rotation angle |

## Behavior

The tooltip appears on hover/focus of the trigger button with a scale + opacity transition. The arrow direction is controlled via `--arrow-angle`.
