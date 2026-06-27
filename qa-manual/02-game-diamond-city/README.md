# Mobile Game — Diamond City (Test Task)

A real test task: I tested an idle/tycoon mobile game and received a detailed
review from the team lead. This folder shows the **corrected version** with the
feedback addressed — to demonstrate how I work with review comments.

## What was reviewed → what I improved
- **GDD review** — kept (done correctly): clarifying questions + found inconsistencies.
- **Checklist** — restructured into blocks + status, merged expected result into the
  check, added negative & boundary checks.
- **Test cases** — expected result per step, added preconditions, deeper coverage
  (e.g. verifying income on train arrival, exact timing from last train sent).
- **Bug reports** — added preconditions, environment (device + OS), app version,
  reproducibility %, detailed steps; corrected overstated priority.
- **Core game loop** — reduced to true loop steps; extra mechanics listed separately.
- **Testing approach** — rewritten by STLC phases.

## Artifacts
- [GDD review](./gdd-review.md) · [Checklist](./checklist.md) · [Test cases](./test-cases.md)
- [Bug reports](./bug-reports.md) · [Testing approach (STLC)](./test-approach-stlc.md)
