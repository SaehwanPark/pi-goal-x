# Fork README Technical Plan

## Scope
- Modify `README.md` to:
  - Remove the upstream npm download ranking badge (which links to the npm package on pi.dev) while keeping the top project logo.
  - Add a clear fork notice below the title referencing the upstream repository `https://github.com/tmonk/pi-goal-x`.
  - Highlight key fork enhancements:
    - Replenishment of wait check allowance on redeclaration to prevent premature exhaustion.
    - Optional `polling.max_checks` with auto-derivation from deadlines.
    - Soft degradation to deadline sleep when check allowance runs out before deadline instead of hard-pausing.
    - Windows and CRLF test suite compatibility.
  - Replace the old `pi install npm:pi-goal-x` instruction with git/source-based installation syntax supported by Pi:
    - Global install: `pi install git:github.com/SaehwanPark/pi-goal-x`
    - Project-local install: `pi install -l git:github.com/SaehwanPark/pi-goal-x`
    - HTTPS install: `pi install https://github.com/SaehwanPark/pi-goal-x`
    - Local clone install: `pi install ./pi-goal-x`
- Verify linting and tests to ensure no regressions.
