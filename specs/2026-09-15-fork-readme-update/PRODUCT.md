# Fork README Update

## Summary

Update `README.md` to reflect that this repository is a fork (`SaehwanPark/pi-goal-x`) of upstream `tmonk/pi-goal-x`. Clarify that installation via npm (`npm:pi-goal-x`) is not valid for this fork, and provide accurate Git- and local-based installation instructions using Pi's package manager.

## Key Changes

1. **Fork Notice & Attribution**: Explicitly state that this repository is a fork of `tmonk/pi-goal-x` with fork-specific enhancements (wait check replenishment, optional max_checks auto-derivation, soft degradation, and Windows test compatibility).
2. **Installation Instructions**: Replace `pi install npm:pi-goal-x` with Git-based installation (`pi install git:github.com/SaehwanPark/pi-goal-x`), HTTPS installation, project-local options (`-l`), and local clone instructions.
3. **Badge & Catalog Link**: Remove or clarify the upstream npm catalog download rank badge which applies to the upstream npm release and not this fork.
