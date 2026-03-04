# Chunk 10 Prompt - Adaptive Orientation and Control Ergonomics

Finalize adaptive layout behavior for portrait and landscape usage.

## Goal
- Keep controls usable and non-intrusive in both orientations, for finger and Apple Pencil workflows.

## Requirements
- In portrait:
  - Keep tool/color rail vertical.
  - Use the full available vertical space for rail content (no arbitrary clipping to a small fixed height).
- In landscape:
  - Reposition picker/tools horizontally in the least intrusive area (typically a bottom strip), preserving canvas focus.
- Ensure selected preset color indicator is reliable and visible across all colors.
- Preserve accessibility metadata and touch target sizing.

## Constraints
- Use SwiftUI-native layout adaptation only (`GeometryReader`, size checks, stacks, scroll views).
- No regression in drawing, undo/redo, smoothing, or performance behavior.

## Acceptance criteria
- Portrait uses full-height vertical control rail.
- Landscape presents horizontal controls that minimize accidental occlusion while drawing.
- Selected color indicator/checkmark appears consistently for all preset colors.
- Build succeeds.

## Output format
- List files added/updated.
- Summarize orientation decision logic in 3-6 bullets.
- Mention any residual UX tradeoffs.
