# Announcement Banner Scroll

A horizontally scrolling announcement banner with seamless loop.

## Usage

```html
<link rel="stylesheet" href="style.css" />

<div class="banner">
  <div class="banner-track">
    <span class="banner-text">Your announcement here →</span>
    <span class="banner-text">Your announcement here →</span>
  </div>
</div>
```

## CSS Custom Properties

| Property | Default | Description |
|---|---|---|
| `--banner-bg` | `#ff6b6b` | Banner background color |
| `--text-color` | `#fff` | Text color |
| `--scroll-duration` | `8s` | Duration for one full scroll cycle |

## Behavior

The track duplicates its content so that as one set scrolls out, the identical set follows seamlessly. The `@keyframes scroll` shifts `translateX` from `0` to `-50%` in a loop.
