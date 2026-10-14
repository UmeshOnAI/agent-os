# Deterministic Hooks Spec

Do not rely on prompt compliance for safety invariants. In Phase 0 (or before any safety-critical work), configure mechanical hooks that hard-block violations:

- File edits outside the worker’s assigned owned_paths.
- `git push --force`, branch switching in the root checkout, or direct pushes to protected branches.
- Shell commands matching destructive or production-mutating patterns.
- Regex matches for secrets, IPs, internal hostnames, or PII in staged diffs or agent reports.

Prefer PreToolUse / PostToolUse hooks, Git pre-commit / pre-push hooks, and CI checks. List which rules remain prose-only.