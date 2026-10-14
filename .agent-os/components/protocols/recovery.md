# Recovery Protocol

On interruption, scheduled wake, or fresh session:

1. Re-inspect actual Git state, open PRs, CI status, running processes, and automation. Compare against the last checkpoint or state.json.
2. Do not repeat an uncertain push, merge, deployment, or external action until its outcome is verified.
3. Continue an existing task with its existing owner, branch, and worktree. Do not create a second owner.
4. If the state is idle, select the next task only within current authority and usage limits.
5. Record the recovery outcome in state.json.

Never assume a prior handover or automation message is current.