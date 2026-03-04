# Chunk 1 Prompt - Canvas Interaction Core

Implement the first working drawing surface using pure SwiftUI.

## Goal
- User can draw on a canvas with touch input.

## Requirements
- Build `DrawingCanvasView` using:
  - `Canvas`
  - `DragGesture(minimumDistance: 0)`
- Maintain an `activeStroke` while dragging.
- Commit stroke into persistent stroke collection on drag end.
- Render both active and committed strokes.

## Constraints
- SwiftUI native components only.
- Keep logic separated between state/store and rendering helpers.
- Avoid premature optimization.

## Acceptance criteria
- Finger drag draws visible lines.
- Drawn lines remain after gesture ends.
- Build passes and no crashes during quick scribbling.

## Output format
- List files added/updated.
- Explain gesture/state flow in concise steps.
- Mention tests added or planned next.
