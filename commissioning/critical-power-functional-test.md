# Critical Power Functional Test — Generic Example

## Purpose
Demonstrate a structured approach for validating a fictional UPS / ATS / generator backup-power sequence before operational handoff.

## Preconditions

- Approved test procedure and change authorization are in place.
- Required stakeholders are present and roles are understood.
- Electrical boundaries and affected loads have been identified.
- Safety requirements and LOTO applicability have been reviewed.
- Backup/redundant capacity is confirmed before testing.
- Abort criteria and recovery steps are understood.

## Functional Test Sequence

| Step | Test Action | Expected Result | Result |
|---|---|---|---|
| 1 | Verify normal source available | ATS indicates normal source healthy | Pass / Fail |
| 2 | Verify UPS normal operation | UPS supports load with no active critical alarm | Pass / Fail |
| 3 | Simulate approved loss of normal source | Backup sequence initiates as designed | Pass / Fail |
| 4 | Observe generator start | Generator reaches stable operating condition | Pass / Fail |
| 5 | Verify transfer | ATS transfers according to approved sequence | Pass / Fail |
| 6 | Verify critical load continuity | UPS maintains downstream critical load | Pass / Fail |
| 7 | Restore normal source | Normal source becomes available and stable | Pass / Fail |
| 8 | Verify retransfer / cooldown | System returns to normal configuration per sequence | Pass / Fail |
| 9 | Review alarms and trends | No unexplained critical alarms remain | Pass / Fail |

## Abort Criteria

Testing should be stopped and escalated if an unexpected condition threatens personnel safety, redundancy, equipment health, or critical-load availability.

## Closeout

- Record test results and exceptions.
- Capture abnormal alarms/events and timestamps.
- Verify equipment is returned to the intended normal configuration.
- Track deficiencies to closure.
- Update documentation only through approved processes.

*This is an educational example and not an operating procedure for any real facility.*
