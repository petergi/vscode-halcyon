# Halcyon Theme

A dark, calming color theme for Visual Studio Code inspired by oceanic twilight.

![VS Code](https://img.shields.io/badge/VS%20Code-1.80+-blue)
![License](https://img.shields.io/badge/license-ISC-green)

## Description

Halcyon is a carefully crafted dark theme featuring soothing blues, cyans, and purples with just enough contrast to keep your eyes comfortable during long coding sessions. The color palette is designed to reduce eye strain while maintaining excellent syntax highlighting clarity.

## Color Palette

<svg viewBox="0 0 700 1100" xmlns="http://www.w3.org/2000/svg">
  <style>
    .category-header { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif; font-size: 18px; font-weight: bold; text-transform: uppercase; fill: #333; letter-spacing: 0.5px; }
    .color-name { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif; font-size: 16px; font-weight: 600; fill: #333; }
    .color-hex { font-family: 'SF Mono', 'Monaco', 'Courier New', monospace; font-size: 14px; fill: #666; }
    .color-usage { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif; font-size: 13px; fill: #888; }
    .divider { stroke: #e0e0e0; stroke-width: 1; }
  </style>

  <!-- Base Colors -->
  <text x="0" y="25" class="category-header">Base Colors</text>
  <line x1="0" y1="35" x2="700" y2="35" class="divider"/>

  <rect x="0" y="55" width="50" height="50" fill="#1D2433" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="75" class="color-name">Editor Background</text>
  <text x="65" y="93" class="color-hex">#1D2433</text>
  <text x="65" y="108" class="color-usage">Main editor background</text>

  <rect x="0" y="125" width="50" height="50" fill="#A2AABC" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="145" class="color-name">Editor Foreground</text>
  <text x="65" y="163" class="color-hex">#A2AABC</text>
  <text x="65" y="178" class="color-usage">Default text color</text>

  <rect x="0" y="195" width="50" height="50" fill="#171C28" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="215" class="color-name">Sidebar Background</text>
  <text x="65" y="233" class="color-hex">#171C28</text>
  <text x="65" y="248" class="color-usage">Sidebar and activity bar</text>

  <rect x="0" y="265" width="50" height="50" fill="#8695B7" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="285" class="color-name">Comments</text>
  <text x="65" y="303" class="color-hex">#8695B7</text>
  <text x="65" y="318" class="color-usage">Comment text (italic)</text>

  <!-- Accent Colors -->
  <text x="0" y="370" class="category-header">Accent Colors</text>
  <line x1="0" y1="380" x2="700" y2="380" class="divider"/>

  <rect x="0" y="400" width="50" height="50" fill="#5CCFE6" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="420" class="color-name">Cyan</text>
  <text x="65" y="438" class="color-hex">#5CCFE6</text>
  <text x="65" y="453" class="color-usage">Functions, classes, links, focus border</text>

  <rect x="0" y="470" width="50" height="50" fill="#BAE67E" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="490" class="color-name">Green</text>
  <text x="65" y="508" class="color-hex">#BAE67E</text>
  <text x="65" y="523" class="color-usage">Strings, markdown code</text>

  <rect x="0" y="540" width="50" height="50" fill="#FFD580" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="560" class="color-name">Yellow</text>
  <text x="65" y="578" class="color-hex">#FFD580</text>
  <text x="65" y="593" class="color-usage">Classes, attributes</text>

  <rect x="0" y="610" width="50" height="50" fill="#FFAE57" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="630" class="color-name">Orange</text>
  <text x="65" y="648" class="color-hex">#FFAE57</text>
  <text x="65" y="663" class="color-usage">Numbers, parameters</text>

  <rect x="0" y="680" width="50" height="50" fill="#C3A6FF" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="700" class="color-name">Purple</text>
  <text x="65" y="718" class="color-hex">#C3A6FF</text>
  <text x="65" y="733" class="color-usage">Keywords, constants</text>

  <rect x="0" y="750" width="50" height="50" fill="#F95972" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="770" class="color-name">Red/Coral</text>
  <text x="65" y="788" class="color-hex">#F95972</text>
  <text x="65" y="803" class="color-usage">Errors, badges, alerts</text>

  <rect x="0" y="820" width="50" height="50" fill="#FFCC66" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="840" class="color-name">Cursor Yellow</text>
  <text x="65" y="858" class="color-hex">#FFCC66</text>
  <text x="65" y="873" class="color-usage">Editor cursor</text>

  <!-- Terminal Colors -->
  <text x="0" y="925" class="category-header">Terminal Colors</text>
  <line x1="0" y1="935" x2="700" y2="935" class="divider"/>

  <rect x="0" y="955" width="50" height="50" fill="#8FD4BE" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="975" class="color-name">Terminal Green</text>
  <text x="65" y="993" class="color-hex">#8FD4BE</text>
  <text x="65" y="1008" class="color-usage">ANSI green</text>

  <rect x="0" y="1025" width="50" height="50" fill="#EF6B73" rx="4" stroke="#d0d0d0" stroke-width="1"/>
  <text x="65" y="1045" class="color-name">Terminal Red</text>
  <text x="65" y="1063" class="color-hex">#EF6B73</text>
  <text x="65" y="1078" class="color-usage">ANSI red</text>
</svg>

## Installation

### From VS Code Marketplace

1. Open VS Code
2. Go to Extensions (Cmd+Shift+X / Ctrl+Shift+X)
3. Search for "Halcyon Theme"
4. Click Install
5. Select the theme: Cmd+K Cmd+T / Ctrl+K Ctrl+T and choose "Halcyon Theme"

### Manual Installation

1. Clone or download this repository
2. Copy the folder to your VS Code extensions directory:
   - **macOS/Linux**: `~/.vscode/extensions/`
   - **Windows**: `%USERPROFILE%\.vscode\extensions\`
3. Reload VS Code
4. Select the theme: Cmd+K Cmd+T / Ctrl+K Ctrl+T and choose "Halcyon Theme"

## Development

Want to customize the theme?

1. Clone this repository
2. Open the folder in VS Code
3. Press **F5** to launch Extension Development Host
4. Edit `themes/Halcyon.json` to modify colors
5. Reload the Extension Development Host (Cmd+R / Ctrl+R) to see changes

## Screenshots

*Note: Will at some point -> Add screenshots of the theme in action with different languages*

## Supported Languages

Halcyon provides enhanced syntax highlighting for:
- JavaScript/TypeScript
- Python
- HTML/CSS
- JSON
- Markdown
- And many more!

## Recommended Settings

For the best experience with Halcyon, consider these settings:

```json
{
  "editor.fontFamily": "JetBrains Mono, Fira Code, Consolas, monospace",
  "editor.fontSize": 14,
  "editor.lineHeight": 1.6,
  "editor.fontLigatures": true,
  "editor.cursorBlinking": "smooth",
  "editor.cursorSmoothCaretAnimation": "on"
}
```

## Credits

Created by Peter Giannopoulos

## License

ISC License - see LICENSE file for details

## Contributing

Found a bug or have a suggestion? Please open an issue on GitHub!

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for version history.
