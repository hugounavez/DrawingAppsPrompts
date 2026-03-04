# Chunk 2 Prompt - Path Smoothing Engine

Upgrade stroke rendering quality by adding Bezier smoothing.

## Goal
- Replace jagged polyline rendering with smoother curves.

## Requirements
- Implement `StrokePathBuilder` that converts `[CGPoint]` into a smoothed `Path`.
- Use midpoint quadratic Bezier interpolation (or equivalent stable smoothing strategy).
- Handle edge cases:
  - 0 points
  - 1 point
  - 2 points
- Integrate builder into existing canvas rendering.

## Constraints
- Keep algorithm deterministic and unit-testable.
- Avoid UI coupling in path-building code.

## Acceptance criteria
- Curves are visibly smoother than raw segment chains.
- Unit tests cover edge cases and representative normal paths.
- Existing drawing behavior remains stable.

## Output format
- List files added/updated.
- Summarize smoothing algorithm in 4-8 bullets.
- Provide test coverage summary.
