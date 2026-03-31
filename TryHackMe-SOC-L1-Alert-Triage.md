# TryHackMe – SOC L1 Alert Triage

**Path:** Junior Security Analyst Intro – SOC L1 Alert Triage  
**Platform:** TryHackMe  
**Focus:** Alert lifecycle, prioritization, and practical triage workflow for SOC L1 analysts.

---

## What was covered

### Task 1 – Introduction to alerts
- Alerts are the practical entry point for SOC operations: they convert suspicious activity into actionable work.
- How alerts are handled (or ignored) directly impacts whether threats are contained early or missed.
- Introduced SOC dashboard context and L1 analyst responsibility in first-line triage.

### Task 2 – Events vs alerts and SOC roles
- **Event:** any logged activity (login, download, process execution, etc.).
- **Alert:** generated when detection logic flags potentially suspicious behavior.
- SOC teams rely on tooling (SIEM, EDR, SOAR) to reduce manual log-review overhead.

Role split in triage ecosystem:
- **L1 analysts:** first review, validation, triage
- **L2 analysts:** deeper investigation and response
- **Detection/security engineers:** rule tuning and detection improvements
- **SOC managers/leads:** quality, prioritization, and process control

**Key takeaway:** alerting filters massive event volume into manageable security decisions.

### Task 3 – Dashboard handling basics
- Real dashboards present alerts by severity and status.
- Typical severity levels: **Low / Medium / High / Critical**.
- Analysts classify outcomes such as **True Positive** or **False Positive**.
- Operational discipline matters: pick/assign alerts and move them out of passive states (e.g., "Awaiting action").

### Task 4 – Prioritization logic
- Triage order should be deliberate, not random.

Practical ordering:
1. Skip alerts already owned/in progress.
2. Prioritize by severity (Critical → High → Medium → Low).
3. Within same severity, handle older alerts first to reduce dwell time.

**Key takeaway:** not all alerts are equal; correct ordering lowers real risk faster.

### Task 5 – End-to-end alert triage workflow
- Claim/assign alert.
- Move to **In Progress**.
- Review core context (user, host, IP, process, timeline).
- Follow playbook/runbook when available.
- Investigate supporting telemetry in SIEM/EDR.
- Decide **True Positive** vs **False Positive**.
- Escalate to L2/IR when needed, or close with reason.

The module also reinforced using environment context and threat intelligence to avoid shallow conclusions.

### Task 6 – Conclusion
- Strong triage is a core L1 skill: fast, accurate decisions with clear escalation.
- Closing an alert is not "the whole incident response," but it is a critical control point in the response chain.

---

## What I learned

- The event/alert distinction is foundational: alerts are prioritized hypotheses, not final verdicts.
- Triage quality depends on both **speed** and **decision accuracy** (especially TP/FP classification).
- Good L1 work is process-driven: ownership, status movement, evidence review, and clean escalation.
- Prioritization discipline (severity + age) reduces time-to-response on meaningful threats.

---

## Takeaways

1. **Alert triage is decision-making under pressure**—methodical workflow beats intuition-only handling.
2. **Status hygiene matters operationally**—unowned or stale alerts create blind spots.
3. **Escalation quality is part of L1 performance**—clear evidence and context make L2 faster and more effective.

---

*Part of the TryHackMe Junior Security Analyst Intro path.*

