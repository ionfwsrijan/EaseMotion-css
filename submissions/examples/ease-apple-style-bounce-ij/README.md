# Apple Style Bounce

An elastic bounce animation inspired by Apple's rubber-band physics.

## Usage

```html
<link rel="stylesheet" href="style.css" />

<div class="bounce-scene">
  <div class="bounce-object">🍎</div>
  <div class="bounce-shadow"></div>
</div>
```

## CSS Custom Properties

| Property | Default | Description |
|---|---|---|
| `--object-color` | `#4ecdc4` | Bouncing object background color |
| `--shadow-color` | `#555` | Shadow color |
| `--bounce-duration` | `0.8s` | Duration of one bounce cycle |

## Behavior

The object bounces with squash-and-stretch (scaleX/scaleY) while the shadow pulses in sync. The `apple-bounce` keyframe decays amplitude naturally. Add `.bounce` class to both `.bounce-object` and `.bounce-shadow` to trigger.
