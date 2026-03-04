# Chunk 8 Prompt - Performance and Scalability Pass

Improve rendering efficiency and prepare for future feature growth.

## Goal
- Maintain smooth drawing performance as stroke count increases.

## Requirements
- Profile and identify key hotspots in drawing/render path.
- Add pragmatic optimizations (example: cache built `Path` per stroke when immutable).
- Minimize repeated work during incremental drawing updates.
- Define extension point for alternative drawing backend (future PencilKit integration).

## Constraints
- Do not introduce premature complexity.
- Keep architecture easy to reason about and test.

## Acceptance criteria
- Noticeable responsiveness improvement on larger drawings.
- No regression in correctness of current features.
- Clear abstraction point exists for optional future renderer engine.

## Output format
- List files added/updated.
- Provide before/after observations (qualitative or measured).
- Summarize scalability decisions and tradeoffs.
