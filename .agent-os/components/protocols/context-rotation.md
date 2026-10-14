# Context Rotation Protocol

Never wait for automatic compaction.

If the session exceeds ~40–50% of the model’s context window (or a configured token ceiling), or after completing a wave gate:

1. Flush all live state to state.json and the handover document.
2. Terminate the current session cleanly.
3. Start a fresh zero-context session that rehydrates exclusively from disk artifacts.
4. Increment context_rotations in state.json.

This preserves peak reasoning accuracy.