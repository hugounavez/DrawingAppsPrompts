# Chunk 3 Prompt - Pencil and Eraser Tools

Add tool switching between pencil and eraser in the drawing flow.

## Goal
- User can switch tools and see immediate behavior change.

## Requirements
- Add toolbar/rail control for selecting:
  - `Pencil`
  - `Eraser`
- Tool controls should support icon-first usage (text optional in this chunk).
- Pencil uses current selected color.
- Eraser uses V1 pragmatic erase behavior (background-color overdraw).
- Display selected tool state clearly in UI.

## Constraints
- Keep tool logic in domain/store layer, not hardcoded in view.
- Preserve current drawing and smoothing behavior.

## Acceptance criteria
- Tool switch is responsive and reliable.
- Pencil draws in selected color.
- Eraser visibly removes/overdraws existing marks as designed.

## Output format
- List files added/updated.
- Explain how tool state propagates from UI to rendering.
- Mention known limitations of V1 eraser approach.
