# Provenance and Live Grounding

Before adding a dependency, skill, hook, or MCP server:

1. Confirm the package/publisher identity and download history on the registry.
2. Inspect the exact pinned version in the repo lockfile.
3. Verify method signatures against installed type definitions or live documentation.
4. Run vulnerability audit.
5. Record license and any material exceptions.
6. Prefer no dependency over an unverified one.

Never rely on pre-training memory for third-party library APIs. Frozen-lockfile installs must succeed in CI.