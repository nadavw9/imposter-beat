# Imposter Beat — agent working agreement

This is currently a compact browser game. Keep the process lighter than the product.

## Global workflow pointer

When available, retrieve only task-relevant topics from `/AI-Knowledge/AI_WORKFLOW_KNOWLEDGE.md`, especially UI & browser verification, Deterministic verification, Debugging & evidence preservation, and Definition of Done.

## Rules

- Understand the complete user round/flow before changing game-state logic.
- For ambiguous bugs, reproduce the failing state or interaction before fixing it.
- Visible or interactive changes are not verified from source inspection alone: exercise the real browser path and check representative mobile/desktop layouts, console errors, and state transitions.
- Preserve game-state invariants across restart/new-round/back navigation; avoid fixes that only make one screen look correct while stale state survives underneath.
- Keep changes proportional to the single-file architecture unless evidence shows decomposition is needed.
- Turn recurring regressions into small deterministic checks when practical.

## Done

The requested interaction works from the user's actual entry path, relevant state transitions are coherent, rendered behavior was inspected, and no temporary debug code remains.
