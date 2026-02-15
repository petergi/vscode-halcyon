# README Color Palette Visual Design

**Date:** 2026-02-14
**Status:** Approved

## Overview

Update the Halcyon Theme README to replace the text-based color palette section with an inline SVG visual that showcases the extended color palette (~18 colors) with detailed information for each color.

## Design Decisions

### Format
- **SVG inline in README** - Provides exact color representation, renders perfectly on GitHub, creates professional appearance

### Information Display
- **Detailed format** - Each color shows:
  - Visual swatch (50×50px)
  - Color name
  - Hex code
  - Usage description

### Color Coverage
- **Extended palette** (~18 colors) - Core colors + important UI colors
- Organized into 4 categories:
  1. Base Colors (4) - backgrounds, foreground, comments
  2. Accent Colors (5) - cyan, green, yellow, purple, red
  3. Syntax Highlighting (4) - numbers, cursor, strings, keywords
  4. Terminal Colors (5) - ANSI color variants

### Visual Design

**SVG Specifications:**
- Width: 700px (GitHub README optimal width)
- Height: ~900px (auto-adjusts based on content)
- Responsive via viewBox

**Color Swatch:**
- 50×50px squares with 4px border radius
- 1px border for definition
- Subtle shadow for depth

**Layout:**
- Left-aligned for easy scanning
- 20px spacing between colors
- 40px spacing between categories
- Visual divider lines between categories

**Typography:**
- Category headers: 18px, bold, uppercase
- Color names: 16px, bold
- Hex codes: 14px, monospace
- Usage: 13px, regular

### Implementation Approach

**Single comprehensive SVG** - One cohesive visual with all categories and colors, providing professional appearance and easy maintenance.

**Replacement strategy** - Remove existing bullet list in Color Palette section (lines 12-22), replace with SVG visual.

## Success Criteria

1. README displays color palette visually with accurate color representation
2. All ~18 colors are shown with name, hex code, and usage
3. SVG renders correctly on GitHub
4. Information is easy to scan and understand
5. Professional, polished appearance

## Files Modified

- `README.md` - Replace Color Palette section with SVG visual
