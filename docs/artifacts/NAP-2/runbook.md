# Runbook: <Service/Workflow>

## Purpose
...

## Preconditions
...

## Normal Operation
...

## Failure Modes & Triage
- Symptom:
- Checks:
- Recovery:

## Escalation
...

## References
...

---

# Runbook: Story Verification / Promotion — NAP-2

## Purpose
Operational notes for validating and promoting changes related to:
- NAP-2: View Item Details

## Preconditions
- Story artifacts generated
- GateReport available
- Required environments reachable (DB/test services)

## Normal Operation
1. Run implementation verification gates
2. Review GateReport evidence
3. If pass, proceed to PR/release checklist
4. If fail, inspect blockers and rerun after fixes

## Gate Evidence Preview
- [1] cmd /c echo implementation gate: placeholder => rc=0 (0.02s)
-   "implementation gate: placeholder"

## Failure Modes & Triage
- Gate command fails:
  - Check command path/toolchain installation
  - Check working directory
  - Check test environment variables / DB availability
- Intermittent test failures:
  - Re-run failed test in isolation
  - Capture logs/screenshots and quarantine if non-deterministic

## References
- `docs/artifacts/NAP-2/gate_report.json`
- `docs/artifacts/NAP-2/test_plan.md`
