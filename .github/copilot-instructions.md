# GitHub Copilot Instructions

This file provides guidance to GitHub Copilot when working with code in this repository.

## Project Overview

This is a VS Code color theme extension called "Halcyon Theme". It's a simple extension with no build process or dependencies.

## Project Structure

- `package.json` - VS Code extension manifest that registers the theme
- `themes/Halcyon.json` - Theme color definitions in iTerm2 format

## Color Format

Colors in `themes/Halcyon.json` use standard VS Code theme format with hex colors:

**UI Colors:**
```json
"editor.background": "#1D2433"
```

**Syntax Highlighting:**
```json
{
  "scope": ["comment"],
  "settings": {
    "foreground": "#8695B7",
    "fontStyle": "italic"
  }
}
```

## When Editing Colors

- Use hex color codes: `#RRGGBB` or `#RRGGBBAA` (with alpha)
- For UI colors: add to the `colors` object
- For syntax highlighting: add to the `tokenColors` array with appropriate TextMate scopes
- Maintain consistent formatting with existing color definitions

## Testing Changes

To test theme changes:
1. Press F5 in VS Code to launch Extension Development Host
2. In the new window, use Cmd+K Cmd+T to open theme selector
3. Select "Halcyon Theme" to preview
4. Reload (Cmd+R) to see updates after editing

## No Build Process

This theme has no build step - VS Code reads the JSON directly. Changes to `themes/Halcyon.json` take effect immediately after reloading the Extension Development Host.
