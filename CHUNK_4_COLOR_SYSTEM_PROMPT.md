# Chunk 4 Prompt - Color System

Implement color selection with presets plus custom picker.

## Goal
- User has fast access to up to 12 colors and custom color selection.

## Requirements
- Add 12 preset color swatches.
- Add native SwiftUI `ColorPicker`.
- Selected color must update pencil output immediately.
- Provide visible selected-color indication (not only subtle border color).

## Constraints
- Keep palette logic reusable (`PaletteView` or equivalent).
- Ensure touch-friendly control sizing.

## Acceptance criteria
- Any preset can be selected and used for drawing.
- Custom color from `ColorPicker` is applied to new pencil strokes.
- UI state is consistent after repeated tool/color switches.

## Output format
- List files added/updated.
- Describe state model for current color and presets.
- Mention accessibility handling for color controls.
