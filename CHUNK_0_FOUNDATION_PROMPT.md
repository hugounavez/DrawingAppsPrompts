# Chunk 0 Prompt - Foundation

Implement the foundation layer for a SwiftUI drawing app. Keep this chunk scoped to structure and contracts only; do not implement full drawing behavior yet.

## Goal
- Prepare a scalable, SOLID architecture baseline.

## Requirements
- Create domain models:
  - `Stroke`
  - `DrawingTool` (`pencil`, `eraser`)
  - `DrawingState`
- Create protocol boundaries:
  - `DrawingStoring`
  - `PathBuilding`
  - `StrokeRendering` (extension point for future backends)
- Keep naming and folder layout clean and future-proof.
- Ensure code compiles without changing user-facing behavior.

## Constraints
- SwiftUI native app.
- Readable code with minimal, useful comments only.
- No dead code and no placeholder TODO blocks unless strictly required.

## Acceptance criteria
- Project builds successfully.
- New models/protocols are in place.
- No drawing UX changes yet.

## Output format
- List files added/updated.
- Explain key architectural decisions in 3-6 bullets.
- Mention tests added (if any) and why.
