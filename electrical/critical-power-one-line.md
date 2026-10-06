# Critical Power One-Line & System Overview

## Objective
Demonstrate a simplified understanding of the electrical path used to deliver reliable power to critical IT loads.

## Generic Architecture

```text
                     +--------------------+
                     |   Standby Generator |
                     +----------+---------+
                                |
                                v
+---------+     +-------------+     +-----+------+     +------------+
| Utility | --> | Transformer | --> | MV/LV SWGR | --> |    ATS     |
+---------+     +-------------+     +------------+     +------+-----+
                                                               |
                                                               v
                                                        +------+-----+
                                                        |    UPS     |
                                                        | + Battery  |
                                                        +------+-----+
                                                               |
                                                               v
                                                        +------+-----+
                                                        | PDU / RPP  |
                                                        +------+-----+
                                                               |
                                                               v
                                                        +------+-----+
                                                        |  IT Load   |
                                                        +------------+
```

> Diagram is intentionally simplified and fictional. Real critical facilities may use multiple redundant paths, switchboards, static transfer equipment, busways, and different topology.

## Operational Considerations

1. **Utility / Transformer** — Establishes the normal source and required voltage transformation.
2. **Switchgear** — Provides distribution, protection, isolation, and switching capability.
3. **Generator / ATS** — Provides an alternate source during loss of normal power and supports automatic transfer logic.
4. **UPS + Batteries** — Maintains uninterrupted power during source disturbances and the transition to standby generation.
5. **PDU / RPP** — Distributes conditioned power toward downstream critical loads.
6. **IT Load** — Represents racks, servers, networking equipment, and other critical computing loads.

## What I Would Monitor

- Source voltage and frequency
- Breaker position/status
- UPS input/output status and load percentage
- Battery status
- Generator availability and running status
- ATS source availability and transfer state
- Downstream loading and abnormal alarms

## Engineering Takeaway
Reliable operation depends not only on individual equipment health but also on understanding the complete power path, protection boundaries, redundancy, transfer sequence, and downstream impact before performing switching or maintenance.
