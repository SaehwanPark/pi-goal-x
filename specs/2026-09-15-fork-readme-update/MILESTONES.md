# Milestones: Fork README Update

- [x] Initial specification and technical plan defined.
- [x] Update `README.md` with fork attribution, fork enhancements, and git-based installation instructions:
  - Removed obsolete upstream npm catalog download rank badge.
  - Added clear fork notice referencing upstream `tmonk/pi-goal-x`.
  - Added summary of fork enhancements (replenishment of wait checks on redeclaration, optional `max_checks`, graceful wait degradation, and Windows test compatibility).
  - Replaced npm installation commands with Pi git/source installation commands (`pi install git:github.com/SaehwanPark/pi-goal-x`, local clone, and project-local flags).
  - Updated explicit execution and waiting section to reflect fork's polling check replenishment and soft degradation behavior.
- [x] Run linter and tests to verify documentation changes:
  - `npm run check`: TypeScript type check passed without errors.
  - `npm run lint`: ESLint passed with 0 errors.
  - `npm test`: 945 passed, 0 failed across 72 test files.
