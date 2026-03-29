# NC Theme

A dark theme for [Obsidian](https://obsidian.md) inspired by **Norton Commander** — the iconic DOS file manager.

Softened CGA palette, NC-style UI elements, and an optional CRT monitor effect.

![NC Theme](screenshots/main.png)

## Features

- **Norton Commander color palette** — CGA-inspired colors, softened for modern displays
- **NC-style UI** — sidebar as file panel, tabs as panel headers, status bar as F-key bar
- **NC-style dialogs** — settings and modals styled as DOS dialog boxes (gray background, cyan buttons)
- **Box-drawing decorations** — tab headers with `┌┐` corner characters
- **`►` list markers** — in reading view
- **CRT effects** — optional scanlines, phosphor glow, vignette, and DOS block cursor (requires [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin)
- **Dark mode only** — Norton Commander doesn't do light mode

## Screenshots

### CRT Mode

![CRT Mode](screenshots/crt.png)

## Recommended Font

The screenshots use [Px437 IBM VGA 9x16](https://int10h.org/oldschool-pc-fonts/) — the actual VGA font from the DOS era. Install it for the full NC experience.

**Settings → Appearance → Text font / Monospace font** → `Px437 IBM VGA 9x16`

## CRT Mode

Install the [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin, then:

**Settings → Style Settings → NC Theme → CRT Effects** — toggle on

This enables:
- Scanline overlay
- Phosphor text glow
- Screen vignette (darkened edges)

## Installation

### From Community Themes

1. Open **Settings → Appearance → Themes**
2. Click **Manage** and search for **NC Theme**
3. Click **Install and use**

### Manual

1. Download `theme.css` and `manifest.json` from the [latest release](https://github.com/eliseevilia/obs-nc-theme/releases)
2. Create folder `.obsidian/themes/NC Theme/` in your vault
3. Place both files inside
4. **Settings → Appearance → Theme** → select **NC Theme**

## Development

```bash
# Edit files in src/, then build:
bash build.sh

# Structure:
# src/classic/variables.css  — color palette
# src/base/*.css              — UI components (use CSS variables)
# src/classic/overrides.css   — NC structural styling
# src/crt/effects.css         — CRT effects (toggled via Style Settings)
```

## License

MIT
