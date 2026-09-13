# Large Thumbnail Grid

Large Thumbnail Grid is a task-switcher layout for KDE Plasma 6. It keeps the
look and behavior of KDE's built-in Thumbnail Grid while making each live
window preview substantially larger.

![Large Thumbnail Grid preview](screenshots/large-thumbnail-grid.png)

## Features

- Larger live previews: 22 grid units wide instead of the built-in layout's 16
- Uses up to 80% of the screen height instead of 70%
- Automatically arranges windows into a compact grid
- Supports keyboard navigation, mouse selection, and closing windows
- Follows the active Plasma theme
- Works with KWin on Wayland and X11

## Requirements

- KDE Plasma 6
- KWin 6

The initial release was tested with KWin 6.7.5 on Wayland.

## Installation

### KDE Store

Open **System Settings → Window Management → Task Switcher**, select
**Get New Task Switchers…**, search for **Large Thumbnail Grid**, and install
it.

### Downloaded package

Install the release archive with:

```bash
kpackagetool6 --type=KWin/WindowSwitcher --install LargeThumbnailGrid-1.0.0.zip
```

Then open **System Settings → Window Management → Task Switcher** and choose
**Large Thumbnail Grid** as the visualization.

To upgrade an existing installation:

```bash
kpackagetool6 --type=KWin/WindowSwitcher --upgrade LargeThumbnailGrid-1.0.0.zip
```

To uninstall it:

```bash
kpackagetool6 --type=KWin/WindowSwitcher --remove large_thumbnail_grid
```

## Background and attribution

This package is a deliberately small modification of the Thumbnail Grid layout
shipped with KDE's KWin. The original implementation is by Chris Holland, with
later work by Nate Graham and other KDE contributors. Large Thumbnail Grid
changes the thumbnail width from 16 to 22 Kirigami grid units and raises the
maximum grid height from 70% to 80% of the current screen.

The original copyright notices are retained in `contents/ui/main.qml`.

## License

GPL-2.0-or-later. See [LICENSE](LICENSE).
