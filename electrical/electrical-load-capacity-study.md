# Electrical Load & Capacity Study

## Project Overview

This project demonstrates electrical load and capacity analysis for a fictional mission-critical data center power system.

The objective is to evaluate UPS loading, three-phase electrical demand, available capacity, redundancy, and remaining headroom before additional critical load is introduced.

---

## System Assumptions

| Parameter | Example Value |
|---|---:|
| System Voltage | 480 V, 3-Phase |
| UPS Module Rating | 500 kVA |
| UPS Configuration | 2N |
| Power Factor | 0.95 |
| UPS A Load | 285 kW |
| UPS B Load | 270 kW |
| Proposed Additional Load | 60 kW |

> All ratings and values are fictional and used only for engineering demonstration.

---

## 1. UPS Capacity

For a 500 kVA UPS operating at a 0.95 power factor:

**Real Power Capacity**

P = S × PF

P = 500 kVA × 0.95

**P = 475 kW**

Therefore, each UPS has an example usable real-power capacity of approximately **475 kW** under the stated assumptions.

---

## 2. Existing UPS Loading

### UPS A

Load Percentage:

Load % = (285 kW / 475 kW) × 100

**UPS A Load = 60%**

Available Capacity:

475 kW − 285 kW = **190 kW**

### UPS B

Load Percentage:

Load % = (270 kW / 475 kW) × 100

**UPS B Load ≈ 56.8%**

Available Capacity:

475 kW − 270 kW = **205 kW**

---

## 3. Three-Phase Current Calculation

For a balanced three-phase system:

**P = √3 × V × I × PF**

Therefore:

**I = P / (√3 × V × PF)**

For UPS A:

I = 285,000 / (√3 × 480 × 0.95)

**I ≈ 361 A**

For UPS B:

I = 270,000 / (√3 × 480 × 0.95)

**I ≈ 342 A**

These calculations demonstrate the relationship between real power, system voltage, current, and power factor in a three-phase electrical system.

---

## 4. Proposed Additional Load

Assume a new **60 kW** critical load is proposed for UPS A.

New UPS A Load:

285 kW + 60 kW = **345 kW**

New Loading Percentage:

(345 kW / 475 kW) × 100

**New UPS A Loading ≈ 72.6%**

Remaining Capacity:

475 kW − 345 kW = **130 kW**

The proposed load therefore remains within the assumed UPS capacity.

However, equipment rating alone should not determine whether a load can be added. Operational limits, redundancy requirements, downstream equipment ratings, protection, phase balance, manufacturer requirements, and site engineering standards must also be evaluated.

---

## 5. Redundancy Evaluation

The example architecture uses a **2N configuration**, where independent A and B power paths support critical loads.

A capacity review should consider:

- Normal operating load
- Available capacity on each power path
- Redundancy requirements
- UPS and downstream PDU ratings
- Breaker and conductor limitations
- Phase loading and imbalance
- Maintenance conditions
- Failure scenarios
- Operational loading limits
- Future capacity requirements

Maintaining electrical headroom helps support reliability, maintenance activities, future expansion, and abnormal operating conditions.

---

## 6. Engineering Assessment

| Metric | UPS A | UPS B |
|---|---:|---:|
| Rated Capacity | 475 kW | 475 kW |
| Existing Load | 285 kW | 270 kW |
| Existing Loading | 60.0% | 56.8% |
| Available Capacity | 190 kW | 205 kW |
| Approx. Current | 361 A | 342 A |
| Proposed Load Addition | +60 kW | — |
| Resulting Load | 345 kW | 270 kW |
| Resulting Loading | 72.6% | 56.8% |
| Remaining Capacity | 130 kW | 205 kW |

---

## 7. Engineering Operations Application

This type of analysis can support engineering operations when evaluating:

- Capacity before adding critical equipment
- UPS and PDU loading
- Electrical system headroom
- Power-path redundancy
- Abnormal loading conditions
- Expansion planning
- Electrical troubleshooting
- Commissioning and load verification

BMS/EPMS data can also be used to compare calculated expectations with actual system loading and operating trends.

---

## Key Skills Demonstrated

- Three-Phase Power Calculations
- UPS Capacity Analysis
- kW / kVA / Power Factor
- Electrical Load Analysis
- Critical Power Distribution
- Capacity Planning
- 2N Redundancy
- BMS/EPMS Data Interpretation
- Engineering Operations
- Critical Infrastructure Reliability

---

> **Portfolio Notice:** This project is an independently created fictional engineering example. All equipment ratings, system configurations, loads, calculations, and scenarios are for educational and portfolio demonstration purposes only. They do not represent any employer, customer, facility, or actual data center configuration.
