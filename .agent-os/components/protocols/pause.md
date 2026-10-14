# Pause Protocol

When the owner says pause, or when a usage window reaches the hard limit:

1. Finish the current safe operation if appropriate.
2. Leave a recoverable checkpoint (state.json + handover note).
3. Pause any automation or heartbeat that would start new work.
4. Record the pause reason and resume steps in state.json.

Do not start new tasks while paused.