# TryHackMe – Junior Security Analyst Intro (Room 4: Systems as Attack Vectors)

**Room:** Junior Security Analyst Intro – Room 4 (Systems as Attack Vectors)  
**Platform:** TryHackMe  
**Focus:** How hosts, servers, and platforms are targeted directly (not only via users), and how analysts think about defense.

---

## What the room covered

### Task 1 – Introduction
- Systems themselves can be primary targets, not just people in the loop.
- SOC analysts benefit from understanding *how* systems are attacked, *why* attackers prioritize certain assets, and what defense looks like in practice.

### Task 2 – Why systems matter to attackers
- Systems (servers, laptops, cloud platforms) hold valuable data and can sometimes be compromised with little or no user “click.”
- Framing: systems are a core part of the “fortress”—compromising a critical system can grant wide control.

Examples of **value to attackers**:
- Personal laptop → botnet recruit, limited data theft
- Admin laptop → pivot into internal trust zones
- Mail server → large-scale email exposure
- Core server → broad impact (e.g., ransomware, full-network leverage)

**Concept checks**
- Can attacks happen without user interaction? **Yes.**
- Can one system breach cause major damage? **Yes.**

### Task 3 – How system attacks tend to progress
- Typical arc: gain access → move toward goal (exfiltration, ransomware, destruction, etc.).

Common starting points:
- **Human-assisted:** weak passwords, malware from downloads, malicious USB
- **Vulnerabilities:** exploitable flaws; unpatched systems are high risk
- **Supply chain:** malicious or compromised trusted components spread widely

**Vocabulary**
- **Vulnerability:** a flaw that can be exploited
- **Supply chain attack:** abuse of trust in software/vendors/components to reach many systems

### Task 4 – CVEs, disclosure, and patching race
- Vulnerabilities are tracked (e.g., **CVE** — Common Vulnerabilities and Exposures).
- Some issues exist undisclosed for a long time (**zero-days** until public); disclosure starts a race between attackers and defenders.

Response themes:
- Patch as soon as safely possible
- Reduce exposure (least privilege, segmentation, hardening)
- Inline controls (IPS/WAF where appropriate)
- Monitoring for exploitation indicators

### Task 5 – Misconfigurations vs vulnerabilities
- **Misconfiguration:** a setup mistake, not the same as a software bug; very common and sometimes easier to abuse than a fresh CVE.

Examples:
- Weak or default credentials
- Overly open access to sensitive systems
- Security controls disabled or poorly tuned

Improvement activities:
- Penetration testing (ethical)
- Vulnerability scanning
- Configuration audits / baselines (e.g., CIS-style guidance)

**Key distinction:** misconfigurations are not “fixed by an update” alone—they need correct design and ongoing governance.

### Task 6 – Real-world defense patterns
- Attackers take the easiest viable path—technical flaws *or* operational mistakes.

Defense layers (examples):
- **Patch management** → reduce exploitable attack surface
- **Training / process** → fewer misconfigurations and safer operations
- **Network protections** → restrict flows and trusted boundaries
- **Antivirus / EDR** → detect and contain execution

Emphasis on **mitigation + detection**: prevent what you can; monitor and respond for what slips through.

### Task 7 – Conclusion
- Even if analysts do not “own” every system, **system-level attack knowledge** improves triage, escalation, and communication with IT/infra teams.
- Effective analysts stay current on threats and share learnings with the team.

---

## What I learned

- Not every serious incident starts with phishing—**systems and services** are direct targets too.
- **Vulnerabilities, misconfigurations, and supply chain** are three different problem classes that need different playbooks.
- **CVE awareness and patch velocity** matter, but **visibility** (logs, detections, investigations) closes the gap when patching lags.
- Analyst value includes connecting alerts to **asset criticality** (what broke, what it can access, what’s next).

---

## Takeaways

1. **Asset context drives severity**—the same technique on a workstation vs a domain controller is not the same incident.
2. **Harden + patch + detect** is a bundle: hardening reduces noise, patching reduces exploitability, detection catches residual risk.
3. **Misconfigurations are operational debt**—they show up in audits, pen tests, and weird auth/network paths long before a CVE headline.

---

*Part of the TryHackMe Junior Security Analyst Intro path. Writeup: Room 4 (Systems as Attack Vectors).*
