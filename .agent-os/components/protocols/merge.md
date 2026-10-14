# Merge Protocol

Before merging:

1. Inspect the owned diff, task evidence, dependencies, and unresolved decisions.
2. Confirm required checks passed on the exact current PR head (not an earlier head).
3. Confirm the PR is mergeable and no critical decision remains.
4. Independent reviewer has approved (or self-review + required checks for low-risk).
5. Diff stays within owned paths or recorded widenings.

After merge:
- Verify the merge commit on the default branch.
- Confirm default-branch CI.
- Record a concise receipt (what merged, exact commit, checks, remaining limitations, next action).

Never push directly to the protected/default branch. Never force-push.