# ease-date-range-picker-slide

A dual-calendar date range picker with a smooth slide animation when navigating between months. Click a start date and then an end date to highlight the selected range.

## Features

- Dual calendar display (current month + next month)
- Range selection: click start date, then click end date
- Selected range highlighted with distinct background
- Start and end dates styled with pill-end rounding
- Month navigation slides the calendars using CSS `transform` transitions
- Previous / next month buttons with animated slide effect
- All CSS custom properties for easy theming

## CSS Custom Properties

| Property | Default | Description |
|---|---|---|
| `--drps-primary` | `#4f6ef7` | Primary brand color for selected dates |
| `--drps-range-bg` | `#dce1fd` | Background for dates in the selected range |
| `--drps-range-border` | `#b3befa` | Hover background for range cells |
| `--drps-cell-size` | `40px` | Height of each date cell |
| `--drps-radius` | `10px` | Outer border radius of the picker card |
| `--drps-shadow` | `0 6px 30px ...` | Box shadow on the picker card |

## Usage

Open `demo.html` in a browser. Click any date to set it as the start of the range, then click another date to complete the range. Use the left/right arrow buttons to navigate months – the calendars slide in from the adjacent direction.
