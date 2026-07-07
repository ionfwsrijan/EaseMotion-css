# App Launcher Grid

A grid of app icons that bounce in with staggered timing.

## Usage

```html
<link rel="stylesheet" href="style.css" />

<div class="launcher-grid animate">
  <div class="app-icon" style="--i: 0">📱</div>
  <div class="app-icon" style="--i: 1">📷</div>
  <div class="app-icon" style="--i: 2">🎵</div>
</div>
```

## CSS Custom Properties

| Property | Default | Description |
|---|---|---|
| `--grid-bg` | `#1a1a2e` | Grid container background |
| `--icon-bg` | `#2d2d44` | Icon tile background |
| `--bounce-duration` | `0.4s` | Duration of each icon's bounce-in |

## Behavior

Each icon receives a staggered delay via `--i` (set inline). The `bounce-in` keyframe scales from 0 → 1.15 → 1 with a cubic-bezier overshoot. Add `.animate` class to trigger.
