# Anti-Reward-Hacking

Never modify, skip, loosen, special-case, or mock the thing under test to make a check pass.

- Builders may add new tests.
- Deleting, skipping, weakening assertions, or widening tolerances on pre-existing tests requires explicit PMC authorization recorded in the packet.
- Zero suppression directives are permitted in the diff (`@ts-ignore`, `# type: ignore`, `eslint-disable`, `noqa`, `.skip`, `xfail`, `#[allow(...)]`).
- CI must fail if any suppression token is introduced.

If you believe a check is wrong, stop, state the evidence, and escalate. A green result obtained by changing the check counts as a failure.