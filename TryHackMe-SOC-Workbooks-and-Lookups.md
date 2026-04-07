# TryHackMe – SOC Workbooks and Lookups

**Path:** SOC Level 1 (Blue Team / SOC Operations)  
**Platform:** TryHackMe  
**Focus:** Using lookups (identity, assets, network context) and workbooks (structured runbooks) to improve triage quality, speed, and consistency.

---

## What was covered

### Task 1 – Introduction
- Alerts alone are not enough for good decisions. Analysts need context about users, systems, and network behavior.
- The room introduces two core ideas:
  - **Lookups**: structured context sources
  - **Workbooks**: step-by-step investigation workflows
- Goal: reduce missed details and make triage repeatable across analysts.

### Task 2 – Identity and asset inventory
- **Identity inventory (Who):** user/account context such as username, role, location pattern, and privilege level.
- **Asset inventory (What):** system context such as host type, criticality, and network placement.
- Practical checks:
  - Should this user access this system?
  - Is the login location/time expected?
  - Is the target a high-value or sensitive asset?
- Typical data sources:
  - Active Directory / Entra ID
  - SIEM / EDR
  - HR and internal CMDB/documentation

**Key takeaway:** without solid "who" and "what" context, triage quality drops and false decisions increase.

### Task 3 – Network diagrams and attack paths
- Network diagrams turn raw logs into understandable attack movement.
- They help map:
  - external IP to entry point
  - subnet boundaries
  - exposed services and likely blast radius
- Example storyline in the room:
  - external actor reaches VPN service (port 10443),
  - gains access,
  - receives internal IP,
  - scans sensitive internal subnets.

**Key takeaway:** diagrams help analysts explain **how** an attacker moved, not just **that** activity happened.

### Task 4 – Workbooks (playbooks/runbooks)
- Workbooks standardize investigations and reduce guesswork.
- Common 3-stage flow:
  1. **Enrichment**: gather user/IP/asset context and TI signals
  2. **Investigation**: correlate SIEM/EDR activity and timeline
  3. **Escalation**: decide TP/FP and handoff path
- Benefits:
  - consistent handling across analysts
  - faster triage
  - fewer process mistakes

### Task 5 – Practical workbook use (malicious email scenario)
- The room walks a realistic process for suspicious email with attachment:
  - collect message and recipient evidence
  - validate sender/authentication (SPF, DKIM, DMARC)
  - assess attachment (sandbox/manual checks)
  - review user activity after delivery/open
  - contain (block), notify, report, escalate when needed

**Key takeaway:** complex cases become manageable when broken into structured steps.

### Task 6 – Conclusion
- Effective SOC L1 analysis combines:
  - **Lookups** for context
  - **Workbooks** for structure
  - **Analyst judgement** for final decisions

---

## What I learned

- Context quality (identity/asset/network) directly affects triage accuracy.
- A workbook is a force multiplier: it preserves quality under pressure and high alert volume.
- Clear process makes handoffs to L2 faster and cleaner.
- Network context is essential for identifying lateral movement and potential impact.

---

## Takeaways

1. **Context before verdict**: don’t classify alerts without identity and asset checks.
2. **Follow the workbook**: structured triage beats intuition-only response.
3. **Tell the attack story**: combine logs + topology to explain path, intent, and risk.

---

*Part of the TryHackMe SOC Level 1 path.*
