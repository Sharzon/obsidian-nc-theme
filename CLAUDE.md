# NC Theme — Obsidian CSS Theme

Norton Commander-inspired dark theme for Obsidian.

## Build

```bash
bash build.sh
```

Concatenates CSS from `src/` into `theme.css`. Order: variables → base → overrides → CRT.

## Structure

- `src/classic/variables.css` — CSS custom properties
- `src/base/*.css` — core component styles (numbered for load order)
- `src/classic/overrides.css` — classic variant overrides with `!important`
- `src/crt/effects.css` — CRT scanline effect (toggled via Style Settings)
- `theme.css` — built output, do not edit directly

## Rules

- **No docs/**: do not create documentation markdown files in this project. Research goes to ai-vault.
- **Always rebuild** after CSS changes: `bash build.sh`
- Commit messages in English.
- Check color contrast with tools, not by eye.
