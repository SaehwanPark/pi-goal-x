# Sync Fork with Upstream

## Summary

Sync the `SaehwanPark/pi-goal-x` fork with the original upstream repository `tmonk/pi-goal-x` (up through upstream's `v0.31.5` release), resolving conflicts while preserving fork-specific enhancements and documentation attribution.

## Scope & Intent

1. **Incorporate Upstream Features**:
   - Merge upstream `main` (commits up to `5a7c4cd`, including PR #64 and PR #65).
   - Adopt upstream's restoration of implicit continuation by default and opt-in execution contracts (`strictExecutionContract: true`).
   - Adopt upstream's updated release assets, docs, and settings options (`explicit execution contracts`).

2. **Preserve Fork Enhancements**:
   - Retain replenishment of wait check allowance on redeclaration and optional `max_checks` calculation from deadline.
   - Retain graceful degradation where exhausted polling checks sleep to deadline rather than hard-pausing.
   - Retain cross-platform test runner fixes (Windows path normalization and CRLF handling).
   - Retain fork attribution and Git-based installation guide in `README.md` (no npm catalog download ranking badge for the fork).

3. **Conflict Resolution**:
   - `README.md`: Keep fork branding, fork notice, fork enhancements, and git-based install guide while integrating upstream's updated settings table and documentation for automatic continuation / optional execution contracts.
   - `extensions/goal-core-tools.ts`: Combine upstream's `strictExecutionContract` note and prompt snippet with the fork's optional `max_checks` schema and auto-derived deadline check documentation.
