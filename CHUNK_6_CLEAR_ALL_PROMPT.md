# Chunk 6 Prompt - Clear All

Add a full-canvas reset action that can be undone.

## Goal
- User can erase entire drawing and start over quickly.

## Requirements
- Add `Clear All` control in toolbar.
- Use a trash icon treatment that is easy to understand.
- Clear action removes all committed and active strokes.
- Register clear operation in undo history so user can restore prior drawing.
- Optional: lightweight confirmation if UX deems it necessary.

## Constraints
- Keep operation atomic and predictable.
- Do not break existing undo/redo semantics.

## Acceptance criteria
- Clear immediately empties canvas.
- Undo after clear restores full previous drawing.
- Works correctly after multiple clear/undo/redo cycles.

## Output format
- List files added/updated.
- Explain clear-all command flow and undo integration.
- Note any UX tradeoff (confirmation vs one-tap action).
