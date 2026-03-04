Prompt to order agent task execution:
```
Build the SwiftUI drawing app by following the existing docs.

Read first

CODEX_IMPLEMENTATION_PROMPT.md (source of truth)

Every file in agent_tasks/ (execute in filename order)

How to execute

For each agent_tasks/*.md in order:

Read task → implement exactly what it asks (consistent with foundation doc).

Ensure the project builds; run basic sanity check if applicable.

Reply with: completed task name + changed files + brief notes.

Rules

Foundation doc overrides task docs if there’s a conflict (note it).

SwiftUI-native UI only (minor tweaks allowed). No third-party libs.

Must include: pencil+eraser, 12 colors + color picker + selected color indicator, undo/redo stack (>=5), clear-all trash icon, app title, HIG/accessibility, scalable clean architecture.

Start now: read the foundation doc, then run tasks sequentially.
```
