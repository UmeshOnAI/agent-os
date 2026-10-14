# Component Index

Load a component only when the task matches its trigger. Prefer the lightest set that covers the risk.

| Component | Path | Trigger |
|-----------|------|---------|
| Recovery protocol | components/protocols/recovery.md | Interrupted session, stale checkpoint, uncertain external action |
| Merge protocol | components/protocols/merge.md | Preparing or executing a merge |
| Review protocol | components/protocols/review.md | Reviewing a PR or preparing self-review |
| Pause protocol | components/protocols/pause.md | Owner says pause or quota/usage limit reached |
| Context rotation | components/protocols/context-rotation.md | Context pressure or long session |
| Anti-reward-hacking | components/guardrails/anti-reward-hacking.md | Any test or check change |
| Circuit breaker | components/guardrails/circuit-breaker.md | Repeated failures inside a worker |
| Hooks spec | components/guardrails/hooks.md | Phase 0 or any safety-critical action |
| Provenance | components/guardrails/provenance.md | Adding a dependency, skill, hook, or MCP |
| Packet skill | components/skills/packet.md | Starting a bounded implementation packet |
| Self-review | components/skills/self-review.md | Before opening or marking a PR ready |
| Architecture checks | components/skills/architecture-checks.md | Structural or boundary changes |
| Outcome validation | components/skills/outcome-validation.md | Milestone or user-facing completion |
| Observability | components/skills/observability.md | Adding logging, tracing, or runtime telemetry |
| Report template | components/templates/report.md | Writing a packet or status report |
| Receipt template | components/templates/receipt.md | After a successful merge |
| Diagnostic note | components/templates/diagnostic-note.md | After circuit breaker trips |
| Protocol regression | components/checks/protocol-regression.md | After material OS or model changes |
| Architecture checks | components/checks/architecture.md | Structural changes or wave gates |