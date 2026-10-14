# Review Protocol

Blocking findings = P0–P2 that cite an authority (requirement, ADR, answered question, or explicit rule).
P3 suggestions go to backlog.

- Max 5 rounds. Rounds ≥2 review only the delta.
- Round 5 escalates to the owner.
- Reviewer must re-run the full check script on the exact PR head before approving.
- Implementing agent produces a structured self-review before the PR is marked ready.

For T3/T4 work, prefer a fresh-context adversarial or property-based pass when practical.