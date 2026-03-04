# Generic Prompt for Codex (Drawing App)

Implement a production-quality iOS drawing app in **pure SwiftUI native components** (minor modifications allowed), following Apple Human Interface Guidelines and SOLID principles.

## Required features
1. A drawing canvas where users can draw with touch.
2. Tool selection: `Pencil` and `Eraser`.
3. Color system:
   - Up to 12 preset colors.
   - A native SwiftUI `ColorPicker` for custom pencil color.
   - A clear visual indicator for the currently selected color.
4. `Undo` and `Redo`.
   - Must support at least **5 consecutive undos**.
5. `Clear All` to erase the full drawing and restart.
   - Use a trash icon control that is visually understandable.
6. App title in the primary toolbar/header.
7. Adaptive layout for both portrait and landscape:
   - Portrait: vertical left rail can use full height.
   - Landscape: controls should switch to a less intrusive horizontal arrangement.

## UX/layout requirements
- Use a drawing-app style layout inspired by common iOS drawing apps (research first, then adapt):
  - Vertical color rail on the **left side**.
  - Tool controls can be icon-only (`Pencil`, `Eraser`) with clear selected-state affordance.
  - Undo/Redo/Clear controls grouped in a clear top action area.
- Keep design SwiftUI-native and avoid custom-heavy rendering controls unless needed.

## Technical constraints
- Use SwiftUI-first APIs for rendering and interaction:
  - `Canvas`, `Path`, `DragGesture(minimumDistance: 0)`, `ColorPicker`, `UndoManager`.
- Do not rely on PencilKit for V1 unless explicitly requested.
- Keep architecture readable, extensible, and scalable:
  - Separate domain models, state/store, rendering logic, and UI components.
  - Prefer protocol-based boundaries for engine/repository style abstractions.
- Follow clean-code standards expected in top-tier engineering teams.

## Implementation quality bar
- Include path smoothing (Bezier-based) so lines are not jagged.
- Add accessibility labels/hints for all controls.
- Ensure control touch targets are at least ~44x44pt.
- Ensure selected states are not color-only.
- Ensure deterministic undo/redo behavior with tests for critical logic.

## Delivery format
1. Implement incrementally in small, reviewable commits/chunks.
2. For each chunk provide:
   - What was implemented.
   - Why the approach was chosen.
   - Tests added/updated.
3. Keep code comments concise and only where logic is non-obvious.

## Optional extension path (not V1)
- Keep rendering abstraction open so a future PencilKit backend can be plugged in without rewriting UI/business logic.
