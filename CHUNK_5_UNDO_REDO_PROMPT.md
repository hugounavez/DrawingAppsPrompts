# Chunk 5 Prompt - Undo and Redo

Implement deterministic undo/redo support for drawing operations.

## Goal
- User can reliably undo and redo edits.

## Requirements
- Integrate `UndoManager` from SwiftUI environment.
- Add Undo/Redo UI controls.
- Register undo actions for:
  - Add stroke
  - Erase action
  - Clear all action (if already implemented)
- Ensure undo depth supports at least **5 consecutive undos**.
- Keep redo stack behavior correct when new edits occur after undo.

## Constraints
- Avoid ad hoc stack logic if `UndoManager` can handle operation registration cleanly.
- Keep command registration centralized (store/controller).

## Acceptance criteria
- Consecutive undo/redo operations are stable and deterministic.
- At least 5 undos work in sequence.
- Button enabled/disabled states reflect actual availability.
- No crashes with rapid repeated taps.

## Output format
- List files added/updated.
- Explain command registration strategy.
- Summarize tests for undo/redo behavior.
