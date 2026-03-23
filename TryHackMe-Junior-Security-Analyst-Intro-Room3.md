# TryHackMe – Junior Security Analyst Intro (Room 3: Humans as Attack Vectors)

**Room:** Junior Security Analyst Intro – Room 3 (Humans as Attack Vectors)  
**Platform:** TryHackMe  
**Focus:** Social engineering, human-centered attack paths, and SOC mitigation/detection mindset.

---

## What the room covered

### Task 1 – Introduction
- Intro to why the human element is often the weakest target in cybersecurity.
- Reinforced SOC analyst context: detection, investigation, and response.

### Task 2 – Why attackers target people
- It is often easier to trick people than bypass hardened infrastructure.
- The room compares organizations to a fortress where humans are gatekeepers.
- Example outcomes of human-targeted compromise:
  - HR account compromise for employee data theft
  - Malware delivery to hijack banking sessions
  - IT admin VPN compromise for internal network access
  - Social engineering of government staff for sensitive information

**Questions and answers**
- What or who is the weakest link in cyber security? **Humans**
- What do attackers seek when targeting humans in a cyberattack? **Access**

### Task 3 – Social engineering methods
- Core concept: victims are manipulated into helping the attacker, often unknowingly.
- Effective social engineering is usually:
  - **Trustworthy** (appears legitimate)
  - **Emotional** (urgency, fear, curiosity)
- Attack types reviewed:
  - Phishing
  - Malware delivery via fake CAPTCHA/QR/search results
  - Deepfakes
  - Impersonation (e.g., fake IT support)
  - USB drops, insider manipulation, fake jobs

### Task 4 – Mitigation vs detection
- Defensive strategy has two parts:
  - **Mitigation:** prevent attacks before execution
  - **Detection:** identify/investigate attacks that bypass controls
- SOC-relevant defensive controls:
  - Anti-phishing filtering
  - Antivirus/EDR
  - "Trust but verify" habits
  - Ongoing user security training

### Task 5 – Practical scenarios
- Applied social engineering concepts in realistic analyst scenarios.
- Identified at-risk users, evaluated threat type, and selected response actions.
- Considered policy improvements to reduce repeat incidents:
  - Better awareness training
  - Stronger authentication
  - Better email filtering and reporting workflows

### Task 6 – Room wrap-up
- Final takeaway: humans remain a primary target, and analyst value comes from recognizing patterns early and coordinating effective response.

---

## What I learned

- Human-focused attacks are often low-cost and high-impact for attackers.
- Social engineering relies more on psychology than technical exploitation.
- Good SOC work combines prevention ideas with fast detection and escalation.
- User awareness and controls (EDR, filtering, MFA habits) reduce both incident count and SOC alert noise.

---

## Takeaways

1. **Access is the attacker objective** in most human-targeted attacks, so monitoring identity/account behavior is critical.
2. **People + process + tooling** is the real defense model: technical controls help, but user behavior and response workflows matter just as much.

---

*Part of the TryHackMe Junior Security Analyst Intro path. Rooms 1–3 now completed with writeups.*

