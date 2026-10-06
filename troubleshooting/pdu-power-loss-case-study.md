# Troubleshooting Case Study — PDU Power Loss

## Scenario
A fictional monitoring system reports loss of input power to a downstream PDU. Some redundancy remains available and the objective is to determine the fault location without creating additional risk.

## Structured Troubleshooting Approach

### 1. Establish impact
- Identify affected equipment and downstream load.
- Determine whether the condition is active.
- Confirm redundancy and whether any critical load is at risk.

### 2. Review the power path
Use the one-line diagram to trace the expected source:

```text
Source -> Switchgear -> UPS -> Distribution -> PDU -> Critical Load
```

### 3. Correlate monitoring data
Review EPMS/BMS status for:
- Upstream source availability
- Breaker status
- UPS output condition
- Related alarms/events
- Event timestamps and sequence

### 4. Field verification
Following approved safety procedures, verify equipment indications and compare them with monitoring-system status. Electrical measurements should only be performed by qualified personnel using approved procedures and appropriate PPE/test equipment.

### 5. Isolate the fault domain
Example logic:
- Upstream source healthy + UPS output healthy + PDU input absent → investigate distribution path between UPS and PDU.
- Upstream abnormalities present → expand investigation toward the source.
- Monitoring status conflicts with field indications → investigate controls, communications, or sensing before assuming a power-system failure.

### 6. Recover and validate
After the issue is corrected through approved procedures:
- Confirm normal equipment state.
- Verify alarms clear appropriately.
- Review trends for stability.
- Confirm redundancy is restored.

## Root-Cause Follow-Up
Document:
- Event timeline
- Initial symptoms
- Fault location
- Contributing factors
- Corrective action
- Preventive action / procedure improvement

## Engineering Takeaway
Effective troubleshooting is systematic: understand impact first, use the one-line to establish the electrical path, correlate monitoring data, verify field conditions safely, isolate the fault domain, and validate recovery before closing the incident.

*Scenario is fictional and contains no production or employer-specific information.*
