# Notification Center Panel

## Description
A slide-out notification center panel that opens from the right side of the screen with a smooth CSS transform transition. Features notification items with icons, timestamps, an unread dot indicator, overlay backdrop, and badge counter on the bell trigger.

## Files
- `demo.html`: HTML structure with bell trigger, slide-out panel, overlay, and notification list. JavaScript toggles `.ncp-open` class.
- `style.css`: CSS with `:root` custom properties, fixed panel with `translateX` transition, item hover highlights, and unread dot indicators.

## How to use
1. Open `demo.html` in your browser and click the bell icon to open the panel.
2. Copy the HTML and CSS into your project.
3. **Structure:**
   - Wrap everything in a `.ncp-container` element
   - Add a `.ncp-bell` trigger button with a badge counter
   - Add a `.ncp-overlay` for the backdrop
   - Add a `.ncp-panel` with header, list of `.ncp-item` elements, and footer
4. **Customization:**
   - **Colors:** Edit the `:root` variables to match your brand palette.
   - **Panel width:** Change `--ncp-width` in `:root`.
   - **Animation speed:** Adjust `--ncp-transition` duration.
   - **Unread state:** Add `.ncp-unread` class to a notification item.
   - **Icons:** Replace the SVG icons inside `.ncp-item-icon` with your own.

## Features
- **Slide-in/out transition:** Panel animates with `transform: translateX` for smooth GPU-accelerated movement
- **Overlay backdrop:** Semi-transparent overlay when panel is open
- **Unread dot indicator:** Blue dot on the left of unread items
- **Badge counter:** Number badge on the bell icon
- **Hover highlight:** Items highlight on hover with a subtle background
- **Escape key close:** Press `Escape` or click overlay/close button to dismiss
- **Responsive:** Full-width panel on mobile screens
- **Google Fonts Inter:** Clean modern typography
- **Pure CSS animations:** JavaScript only handles class toggling

## Use Cases
- App notification centers
- Inbox or message panels
- Activity feeds
- Alert and update dashboards
- Mobile slide-out menus
