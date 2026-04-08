# TryHackMe – SOC Metrics and Objectives

**Path:** SOC Level 1 (SOC Team Internals)  
**Platform:** TryHackMe  
**Focus:** Core SOC performance metrics (MTTD, MTTA, MTTR, FPR, escalation quality, detection quality) and how analysts use them to improve operations.

---

## What was covered

### Task 1 – Why SOC metrics matter
- SOC performance must be measured just like any other operations team.
- Metrics are used to evaluate:
  - detection speed
  - response quality
  - team effectiveness
- Intro metrics included: **MTTD**, **MTTA**, **MTTR**, **SLA**, and **False Positive Rate**.

**Key takeaway:** metrics show how fast and how well a SOC detects and responds to threats.

### Task 2 – Core operational metrics
- **Alerts Count (AC):** total alert volume and workload signal.
  - Very high: analyst overload/noise risk
  - Very low: potential visibility or detection gaps
- **False Positive Rate (FPR):** percent of non-malicious alerts.
  - High FPR increases fatigue and misses
  - 0% is unrealistic in practice
- **Alert Escalation Rate (AER):** share of alerts escalated from L1.
  - Too high may indicate over-escalation
  - Too low may indicate under-escalation/missed threats
- **Threat Detection Rate (TDR):** share of real threats detected.
  - Target is as high as possible
  - Misses can drive major incident impact

**Key takeaway:** SOC quality is a balance problem: reduce noise without missing real attacks.

### Task 3 – Triage timing metrics and SLAs
- **MTTD (Mean Time to Detect):** attack occurrence to alert detection.
- **MTTA (Mean Time to Acknowledge):** alert created to analyst pickup.
- **MTTR (Mean Time to Respond):** analyst pickup to containment/response.
- Flow model:
  - Attack -> Detect (**MTTD**) -> Acknowledge (**MTTA**) -> Respond (**MTTR**)
- Coverage model (24/7 vs 8/5 SOC) directly affects these timings.

**Key takeaway:** faster detection, acknowledgment, and response reduce business impact.

### Task 4 – Improving weak metrics
- If **FPR is high**:
  - tune noisy rules
  - suppress known-benign patterns
  - automate repetitive noise handling
- If **MTTD is high**:
  - improve detection logic
  - ensure logs are real-time and complete
- If **MTTA is high**:
  - improve notification/escalation routing
  - balance team workload
- If **MTTR is high**:
  - escalate earlier
  - use tested workbooks/runbooks

**Key takeaway:** metrics are action signals; each bad metric should map to a concrete operational fix.

### Task 5 – Scenario-based SOC management
- Applied metric thinking to practical SOC management scenarios:
  - delayed response to critical alerts
  - late triage start by L1
  - communication/process breakdowns
- Improvement actions included:
  - better alerting pipeline/notifications
  - engineering automation tasks
  - workbook refinement
  - proper escalation workflow

**Key takeaway:** metrics are not dashboard vanity values—they expose workflow bottlenecks and drive real improvements.

### Task 6 – Conclusion
- Strong SOC analysts understand both:
  - **technical detection work**, and
  - **operational performance measurement**.
- Metrics connect analyst actions to team-level security outcomes.

---

## What I learned

- Good SOC performance is measured, not assumed.
- L1 analyst behavior influences MTTA/MTTR directly.
- Too much noise and too little escalation discipline both harm response quality.
- Workbooks, automation, and rule tuning are the practical levers behind better metrics.

---

## Takeaways

1. **Metrics turn SOC work into measurable operations.**
2. **Every weak metric should produce a concrete improvement action.**
3. **As an L1 analyst, faster and cleaner triage improves team outcomes immediately.**

---

*Part of the TryHackMe SOC Level 1 path.*
