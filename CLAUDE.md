# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a VS Code color theme extension called "Halcyon Theme". It's a simple extension with no build process or dependencies.

## Project Structure

```
halcyon-theme/
├── package.json           # VS Code extension manifest
└── themes/
    └── Halcyon.json       # Theme color definitions
```

## VS Code Theme Architecture

**Extension Manifest** (`package.json`):
- Declares this as a VS Code extension with `engines.vscode`
- Registers the theme under `contributes.themes`
- Sets the base UI theme to `vs-dark`
- Points to the theme JSON file

**Theme File** (`themes/Halcyon.json`):
- Contains all color token definitions in VS Code theme format
- Uses standard hex color codes (e.g., `#1D2433`)
- Two main sections:
  - `colors`: UI colors (editor, sidebar, terminal, etc.)
  - `tokenColors`: Syntax highlighting rules with TextMate scopes

## Development Workflow

**Testing the theme:**
1. Open this directory in VS Code
2. Press F5 to launch Extension Development Host
3. In the new window: Cmd+K Cmd+T to open theme selector
4. Select "Halcyon Theme" to preview changes

**Making color changes:**
1. Edit `themes/Halcyon.json` color definitions
2. Reload the Extension Development Host (Cmd+R) to see changes
3. No build step required - VS Code reads the JSON directly

**Publishing:**
This theme can be published to the VS Code Marketplace using `vsce publish` (requires vsce CLI tool).

## Color Format

Colors in Halcyon.json use standard VS Code format:

**UI Colors** (`colors` object):
```json
{
  "editor.background": "#1D2433",
  "editor.foreground": "#A2AABC"
}
```

**Syntax Highlighting** (`tokenColors` array):
```json
{
  "name": "Comment",
  "scope": ["comment"],
  "settings": {
    "foreground": "#8695B7",
    "fontStyle": "italic"
  }
}
```

All colors use hex format (`#RRGGBB` or `#RRGGBBAA` for alpha).
