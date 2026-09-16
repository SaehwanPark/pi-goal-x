# Milestones: Sync Fork with Upstream

- [x] Configure upstream remote for `https://github.com/tmonk/pi-goal-x.git` and fetch upstream refs.
- [x] Identify divergence: upstream contains PR #64 (implicit continuation restoration and opt-in execution contracts) and PR #65 (v0.31.5 patch release).
- [x] Merge `upstream/main` into local `main`.
- [x] Resolve conflicts:
  - `README.md`: Retained fork header, fork notice, fork enhancements, and git-based installation instructions while incorporating upstream's updated settings documentation and automatic continuation explanation.
  - `extensions/goal-core-tools.ts`: Combined upstream strict contract documentation with fork's auto-derived polling checks and optional `max_checks` schema.
- [x] Verify seamless integration of scheduler changes in `extensions/goal-scheduler.ts` and test coverage in `tests/goal-scheduler.test.ts`.
- [x] Verify codebase integrity:
  - `npm run check`: TypeScript type checking passed cleanly.
  - `npm run lint`: ESLint passed cleanly with 0 errors.
  - `npm test`: 954 unit tests passed across 72 files.
  - `npm run test:integration`: 31 integration tests passed across 5 suites.
  - `npm run test:all`: 1004 total tests passed across 77 files, including real SDK e2e tests.
