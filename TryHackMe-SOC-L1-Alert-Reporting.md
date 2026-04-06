# TryHackMe – SOC L1 Alert Reporting

**Path:** Junior Security Analyst Intro – SOC L1 Alert Reporting  
**Platform:** TryHackMe  
**Focus:** What happens after triage: **reporting**, **escalation**, and **communication** so real threats move to the right people with enough context.

---

## What was covered

### Task 1 – Introduction
- L1 analysts don’t only **classify** alerts—they **report** findings, **escalate** serious issues, and **communicate** across teams.
- Sets up the idea that handling incidents goes beyond “spotting something suspicious.”

### Task 2 – Alert funnel / lifecycle
- Many alerts enter the funnel; **L1** filters most; only a smaller set of meaningful **true positives** may go to **L2** and potentially to **DFIR**.
- Three pillars introduced:
  - **Alert reporting** — documented findings for others
  - **Escalation** — handing serious work up the line (e.g. to L2)
  - **Communication** — coordinating with other teams

**Recall**
- Passing alerts to **L2** is **escalation**.
- Writing detailed findings is **reporting**.

### Task 3 – Writing alert reports
- Good reports let **L2** understand the situation without redoing L1’s work.
- Reports: support **escalation**, preserve a **record**, and sharpen your own **investigation** thinking.
- **5 W’s** framing for clarity:
  - **Who** — affected user / system
  - **What** — action or activity observed
  - **When** — timeline
  - **Where** — system / location / asset
  - **Why** — reasoning and verdict (e.g. TP/FP and basis)

**Key takeaway:** if you can explain the alert clearly, you understand it.

### Task 4 – When and how to escalate
**Escalate when**
- Serious or **confirmed** malicious activity
- **Further action** is needed (e.g. isolation, reset, IR)
- You need **help** or are **unsure**

**Typical flow**
1. Finish your **analysis**
2. **Write the report**
3. **Assign** / route the alert to **L2**
4. L2 continues deeper investigation

**Key takeaway:** escalation gets real threats handled **properly** and **quickly**.

### Task 5 – SOC communication (real situations)
Examples the room emphasized:
- **L2 not responding** → follow org procedure (e.g. further **escalation** chain; not “skip straight to random channels”)
- **Compromised account** → contact the user via **trusted / safe** channels (not the potentially compromised mailbox/system alone)
- **Overwhelmed** → **prioritize** by risk and **tell** L2 / lead as required
- **Mistake made** → **report** it immediately
- **Tools failing** → document what you can, **escalate** the tooling/visibility gap

**Takeaways**
- In **critical** cases, follow the defined **escalation chain** (don’t improvise by going to the “top” first unless policy says so).
- If you think you **missed** something on an attack, **inform** **L2**—covering silence hurts more than correcting fast.

### Task 6 – Conclusion
Three L1 skills reinforced:
1. **Reporting**
2. **Escalation**
3. **Communication**

**Closing idea:** a strong analyst doesn’t only **detect**—they **report**, **escalate**, and **communicate** so the org actually **handles** the threat.

---

## What I learned

- Triage is only half the job; **documentation and handoff** are how organizations scale response.
- The **5 W’s** are a practical checklist so L2 gets **who/what/when/where/why** without guesswork.
- **Escalation** is a **process**, not an admission of failure—especially when stakes or uncertainty are high.
- **Communication** under pressure (volume, outages, mistakes) needs calm **priority** and honest **escalation**.

---

## Takeaways

1. **Report like the next shift depends on it**—because it does.
2. **Escalate on impact and uncertainty**, not only when you “feel finished.”
3. **Use the chain and safe channels** so communication doesn’t make the incident worse.

---

*Part of the TryHackMe Junior Security Analyst / SOC Level 1 path.*
