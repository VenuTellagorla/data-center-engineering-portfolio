# BMS / EPMS Alarm & Trend Analysis

## Scenario
A fictional EPMS alarm indicates that a UPS output parameter has moved outside its normal operating band while the critical load remains online.

## Example Fictional Data

| Time | UPS Load | Output Voltage | Battery State | Alarm State |
|---|---:|---:|---|---|
| 10:00 | 51% | 480 V | Normal | Normal |
| 10:05 | 53% | 479 V | Normal | Normal |
| 10:10 | 55% | 474 V | Normal | Warning |
| 10:15 | 56% | 471 V | Normal | Warning |
| 10:20 | 55% | 479 V | Normal | Cleared |

*Values are fictional and are not operating limits for any real facility.*

## Response Method

1. Acknowledge and identify the affected asset and alarm type.
2. Determine whether the condition is active, intermittent, or already cleared.
3. Review related EPMS/BMS trends instead of evaluating a single data point in isolation.
4. Check upstream and downstream equipment status to determine whether the issue is localized.
5. Confirm whether redundancy remains available and assess potential impact to critical load.
6. Follow approved operational procedures and escalation paths if field verification or intervention is required.
7. Document observations, timeline, actions, and final condition.

## Key Principle
An alarm is a starting point for investigation—not automatically proof of equipment failure. Correlating trends, equipment state, related alarms, and field conditions supports safer and more accurate troubleshooting.
