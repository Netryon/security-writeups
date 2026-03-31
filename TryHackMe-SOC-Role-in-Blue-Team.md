# TryHackMe – Junior Security Analyst Intro (Room 2: SOC Role in Blue Team)

**Room:** Junior Security Analyst Intro – Room 2 (SOC Role in Blue Team)  
**Platform:** TryHackMe  
**Focus:** Blue Team structure, SOC roles, SOC vs MSSP, and role-to-incident assignment.

---

## What the room covered

### Task 1 – Intro to SOC L1
- Overview of what an L1 analyst does.
- Learning goals: understand Blue Team context, where SOC fits in a company, and the L1 career path.
- Prerequisite reminder: Junior Security Analyst Intro + SOC roles/process basics.

### Task 2 – Security hierarchy in organizations
- Different companies have different priorities, so team structures vary.
- Smaller companies may have only IT/InfoSec handling security.
- Larger organizations may include:
  - **Red Team** (offensive testing)
  - **GRC Team** (policy/compliance)
  - **Blue Team** (defensive operations)

**Questions and answers**
- Which senior role typically makes key cyber security decisions? **CISO**
- What is the common name for roles like SOC analysts and engineers? **Blue Team**

### Task 3 – Blue Team roles and escalation path
- Blue Teams may range from a few members to large teams.
- Typical roles:
  - **L1 Analyst**: triage and basic investigation
  - **L2 Analyst**: deeper technical investigations
  - **SOC Engineer**: tool configuration (SIEM/EDR)
  - **Manager**: team coordination/operations
- If incidents exceed SOC capability, organizations escalate to incident response teams such as:
  - **CIRT / CSIRT / CERT**

**Questions and answers**
- Does Blue Team focus on defensive or offensive security? **Defensive**
- Which department handles active or urgent cyber incidents? **CIRT**

### Task 4 – SOC career path and SOC vs MSSP
- SOC L1 is a strong entry point to learn real incidents and workflows.
- Growth path: strengthen core skills, stay current, practice, prepare for interviews, then move toward senior roles (e.g., L2).
- Learned SOC vs MSSP difference:
  - **SOC** = internal team (within a company)
  - **MSSP** = external provider offering security services to clients

**Questions and answers**
- How would you call a cyber security company providing SOC services? **MSSP**
- Which role naturally continues your SOC L1 analyst journey? **SOC L2 Analyst**

### Task 5 – Role assignment simulation
As CISO, assign the correct role to each incident type:

| Scenario | Role |
|---|---|
| SIEM alert triage | Lucas (SOC L1) |
| Phishing malware deep analysis | Susan (SOC L2) |
| Ransomware incident | Robert (CERT Lead) |
| PCI DSS audit | Nick (GRC Auditor) |
| Vulnerability check | Ben (Pentester) |
| SIEM issue | Eugen (SOC Engineer) |
| FIN7 analysis | Alice (Threat Researcher) |

---

## What I learned

- Blue Team is the defensive side of security operations, but not every company has the same structure.
- Correct escalation matters: SOC handles many incidents, but major active incidents can require CIRT/CERT support.
- SOC and MSSP environments differ, and understanding both helps with job targeting.
- SOC L1 is an entry point, not a dead end: there is a clear path to L2 and specialized roles.

---

## Takeaways

1. **Role clarity improves response quality**: knowing who handles triage, deep analysis, tooling, compliance, and incident response reduces confusion during incidents.
2. **Career strategy should match team reality**: apply to both internal SOC and MSSP roles, and build skills that transfer across both environments.

---

*Part of the TryHackMe Junior Security Analyst Intro path. Room 3 writeup to follow.*

