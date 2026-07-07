# Answer Reveal Card

A card that wipes from top to bottom to reveal an answer on click.

## Usage

```html
<link rel="stylesheet" href="style.css" />

<div class="reveal-card" tabindex="0">
  <div class="reveal-card-front">
    <p class="question">Your question here?</p>
    <span class="hint">Click to reveal →</span>
  </div>
  <div class="reveal-card-back">
    <p class="answer">The answer here.</p>
  </div>
</div>

<script>
  document.querySelector('.reveal-card').addEventListener('click', function() {
    this.classList.toggle('revealed');
  });
</script>
```

## CSS Custom Properties

| Property | Default | Description |
|---|---|---|
| `--card-bg` | `#2d2d44` | Front card background color |
| `--reveal-color` | `#4ecdc4` | Back reveal background color |
| `--wipe-duration` | `0.5s` | Wipe animation duration |

## Behavior

Clicking the card toggles the `.revealed` class. The front wipes upward (`inset(0 0 100% 0)`) while the back wipes in from the bottom (`inset(0 0 0 0)`) using `clip-path`.
