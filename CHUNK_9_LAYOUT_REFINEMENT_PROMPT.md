# Chunk 9 Prompt - Layout Refinement and Visual UX

Refine the app shell and control placement based on common iOS drawing app patterns.

## Goal
- Make the layout feel intentional, clear, and drawing-focused.

## Requirements
- Research a few drawing apps and apply only transferable layout patterns.
- Add a top bar with app title and primary actions.
- Move color controls into a left vertical rail (including custom color picker access).
- Keep tool buttons icon-only while preserving clear selected-state affordances.
- Ensure current selected color has an explicit visual indicator.

## Constraints
- Use native SwiftUI components with minor styling only.
- Preserve existing drawing behavior and architecture.

## Acceptance criteria
- Canvas remains the visual focus.
- Left-side color rail is usable on small screens.
- Icon-only tools are understandable via affordances and accessibility metadata.

## Output format
- List files added/updated.
- Cite 2-4 inspiration references and what was adapted.
- Summarize UX tradeoffs taken.
