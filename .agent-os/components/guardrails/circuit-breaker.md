# Circuit Breaker

A worker may attempt at most 3 consecutive code edits to resolve the same failing test, build, or check.

On the third failure:
1. Immediately revert to the last known clean state (`git checkout` or equivalent).
2. Stop writing implementation code.
3. Write a diagnostic note listing the 3 attempted hypotheses, exact failure outputs, and 2 competing root-cause hypotheses.
4. Either run a minimal read-only reproduction script to falsify one hypothesis or halt and escalate to the PMC for model tier upgrade or scope refinement.

Do not start a fourth attempt on the same failure.