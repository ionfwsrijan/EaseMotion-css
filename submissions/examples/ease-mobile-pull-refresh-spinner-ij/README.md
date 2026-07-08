# ease-mobile-pull-refresh-spinner

A circular spinner rotation tied to pull progress. CSS handles visual rotation via the \--pull-progress\ custom property.

## Usage
Open demo.html. Click and drag down on the list area to pull; watch the spinner rotate proportionally. Release past the threshold to trigger the refresh animation.

## Custom Properties
| Property | Default | Description |
|----------|---------|-------------|
| --primary | #4f46e5 | Primary accent color |
| --bg | #f8fafc | Page background |
| --spinner-size | 40px | Spinner diameter |

## Notes
JavaScript sets the \--pull-progress\ variable from drag distance. CSS handles all visual rotation.
