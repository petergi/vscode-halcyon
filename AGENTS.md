# AGENTS.md

This file provides guidance to AI coding agents (Cursor, Windsurf, Cline, Aider, etc.) when working with code in this repository.

## Project Overview

**Halcyon Theme** is a VS Code color theme extension. It's a minimal project with no build process, no dependencies, and no scripts.

## Project Structure

```
halcyon-theme/
├── package.json              # VS Code extension manifest
├── themes/
│   └── Halcyon.json         # Theme color definitions (iTerm2 format)
├── CLAUDE.md                # Claude Code instructions
├── .github/
│   └── copilot-instructions.md   # GitHub Copilot instructions
└── AGENTS.md                # This file
```

## Key Information

### No Build Process
- VS Code loads theme JSON files directly
- No compilation, bundling, or preprocessing required
- Changes to `themes/Halcyon.json` are immediately available after reload

### Color Format
The theme uses **standard VS Code theme format** with hex colors:

```json
{
  "name": "Halcyon",
  "type": "dark",
  "colors": {
    "editor.background": "#1D2433",
    "editor.foreground": "#A2AABC"
  },
  "tokenColors": [
    {
      "scope": ["comment"],
      "settings": {
        "foreground": "#8695B7"
      }
    }
  ]
}
```

**Color values:** Use hex format `#RRGGBB` or `#RRGGBBAA` (with alpha channel).

### Extension Manifest
`package.json` registers the theme under `contributes.themes`:
- `label`: Display name shown in VS Code theme picker
- `uiTheme`: Base theme (`vs-dark` for dark themes)
- `path`: Relative path to theme JSON file

## Development Workflow

### Testing the Theme
1. Open this directory in VS Code
2. Press **F5** to launch Extension Development Host
3. In the new window: **Cmd+K Cmd+T** (or **Ctrl+K Ctrl+T** on Windows/Linux)
4. Select "Halcyon Theme" from the theme picker
5. Make changes to `themes/Halcyon.json`
6. **Cmd+R** (or **Ctrl+R**) in Extension Development Host to reload and see changes

### Making Color Changes

**Adding UI colors:**
Add to the `colors` object:
```json
"editor.lineHighlightBackground": "#29304033"
```

**Adding syntax highlighting:**
Add to the `tokenColors` array:
```json
{
  "name": "My Token",
  "scope": ["entity.name.function"],
  "settings": {
    "foreground": "#5CCFE6",
    "fontStyle": "italic"
  }
}
```

Color format: Hex codes `#RRGGBB` (or `#RRGGBBAA` for transparency)

### Common Theme Elements

The theme JSON contains color definitions for:
- **ANSI colors** (0-15): Terminal colors
- **Background/Foreground**: Main editor colors
- **Cursor colors**: For both light and dark modes
- **Selection colors**: Text selection background
- **Badge colors**: Status bar badges
- **Link colors**: Hyperlinks in terminal

## Publishing

To publish to VS Code Marketplace:
1. Install `vsce`: `npm install -g @vscode/vsce`
2. Package: `vsce package`
3. Publish: `vsce publish`

Requires a publisher account on the VS Code Marketplace.

## Architecture Notes

This is intentionally minimal - there's no complex architecture. The entire theme is defined in a single JSON file that VS Code reads directly.

## Common Tasks

**Add a new color variant:**
1. Duplicate an existing color definition
2. Modify the RGB component values
3. Update the key name to match VS Code's theme API

**Change base colors:**
1. Edit the corresponding color in `themes/Halcyon.json`
2. Remember to update both light and dark variants if they exist
3. Reload Extension Development Host to preview

**Debug color issues:**
- Use VS Code's Developer Tools (Help > Toggle Developer Tools)
- Inspect elements to see which theme token is applied
- Cross-reference with VS Code's theme color reference

## Reference

- [VS Code Theme Guide](https://code.visualstudio.com/api/extension-guides/color-theme)
- [VS Code Theme Color Reference](https://code.visualstudio.com/api/references/theme-color)
