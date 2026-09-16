# Sync Fork with Upstream Technical Plan

## Approach

1. **Remote Configuration & Fetch**:
   - Add upstream remote `https://github.com/tmonk/pi-goal-x.git` (done).
   - Fetch latest upstream branches and tags (`upstream/main` at `5a7c4cd`).

2. **Merge & Conflict Resolution**:
   - Merge `upstream/main` into local `main`.
   - Resolve conflict in `README.md`:
     - Discard upstream npm catalog badge in favor of fork notice and fork enhancements summary.
     - Accept upstream's additions to settings and automatic continuation sections.
     - Retain git-based installation commands.
   - Resolve conflict in `extensions/goal-core-tools.ts`:
     - Retain `update_goal` description mentioning both `strictExecutionContract` opt-in and optional polling checks auto-derived from deadline.
     - Retain upstream's updated promptSnippet: `"Complete, block, pause, or optionally save a scheduling decision."`.
     - Preserve TypeBox parameter schema with `max_checks: Type.Optional(...)`.

3. **Validation**:
   - Verify scheduler logic in `extensions/goal-scheduler.ts` satisfies both upstream implicit continuation / opt-in strict contract and fork check replenishment.
   - Run type checking: `npm run check`.
   - Run linting: `npm run lint`.
   - Run unit and e2e test suites: `npm test`, `npm run test:integration`, and `npm run test:all`.
