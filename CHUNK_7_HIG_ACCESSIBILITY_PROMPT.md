# Chunk 7 Prompt - HIG and Accessibility Hardening

Refine UX quality to align with Apple Human Interface Guidelines and accessibility best practices.

## Goal
- Production-ready interaction quality baseline.

## Requirements
- Ensure interactive controls are touch-friendly (~44x44pt minimum target).
- Add accessibility labels/hints/traits for all drawing controls.
- Ensure selected states are not color-only (shape/icon/border/state text).
- Review contrast in Light and Dark mode.
- Add platform-appropriate keyboard shortcuts for undo/redo where supported.
- Ensure app title is present and announced correctly.

## Constraints
- Preserve current visual language; improve clarity without overdesign.
- Keep all controls SwiftUI-native.

## Acceptance criteria
- VoiceOver identifies and activates all key controls.
- Controls remain usable on small screens.
- Selected states are understandable without relying only on color vision.

## Output format
- List files added/updated.
- Provide a concise HIG/accessibility checklist with pass/fail status.
- Mention any residual gaps and next fixes.
