# TryHackMe – Junior Security Analyst Intro (Room 1)

**Room:** Junior Security Analyst Intro (first of 3 in the path)  
**Platform:** TryHackMe  
**Focus:** SOC role, team structure, and a simulated day-in-the-life alert workflow.

---

## What the room covered

1. **Your role and team** – You play a junior analyst; your team is the SOC team. The room reinforces that you’re part of the Security Operations Center.
2. **SOC team structure** – Introduced roles: Senior Analyst, SOC Engineer, SOC Manager, Incident Responder, and what each typically does. No quiz; informational.
3. **Day in the life** – A simulated alert dashboard with Critical, Medium, and Low alerts. You work through one malicious alert from triage to escalation to firewall block.

---

## What I did (task 3 – the hands-on part)

- **Alert triage:** Opened the simulated dashboard and identified the **malicious** alert. Read the alert message and **copied the IP address** mentioned in it.
- **IP lookup:** Used the “IP Hunter” tab, pasted the IP, and reviewed the result to confirm it was malicious and/or linked to other activity.
- **Escalation:** Escalated to the **SOC Team Lead** (my senior analyst), because for a junior analyst he’s the right person to go to when I need guidance or don’t fully understand something—escalating to the wrong role would have been incorrect.
- **Remediation:** The team lead analyzed the alert and asked me to **block the IP in the firewall**. In the firewall tab I added a **deny rule** for that IP and included a **comment** (e.g. reason or ticket reference).
- **Completion:** Received the completion code and finished the room.

---

## What I learned

- **Alert dashboard:** How a SOC-style dashboard can look—alerts by severity (Critical/Medium/Low) and enough detail in the message to pull IOCs (e.g. IP).
- **SOC roles:** Who’s on the team (Senior Analyst, SOC Engineer, SOC Manager, Incident Responder, Team Lead) and how escalation should go (e.g. junior → team lead when in doubt).
- **Escalation:** As L1, I don’t fix everything myself; I triage, gather info, and escalate to the right person when needed.
- **Firewall block:** A basic “deny” rule: add the malicious IP, add a comment for audit/tracking. Same idea as deny-by-IP in real firewalls (e.g. blocklist).

---

## Takeaways

1. **Triage → Enrich → Escalate → Remediate** is a simple L1 flow: understand the alert, check the IP (or other IOC), escalate if needed, then apply the requested control (e.g. block).
2. **Escalate to the right role** – In a real SOC, wrong escalation wastes time; here, choosing the Team Lead (senior analyst) was correct for a junior.

---

*Part of the TryHackMe Junior Security Analyst path. Room 2 and 3 writeups to follow.*
