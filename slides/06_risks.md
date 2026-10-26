---
marp: true
theme: default

_class: lead
paginate: true
---

# Risks and Responsible Use of Generative AI in research

At the end of this section you will have:
- a framework to think about and discuss risks and mitigation
- strategies to protect yourself and your research
- local sources of information and help

<br/><br/>
<small><sup>These slides are derived from [Code Refinery: Coding with AI, lesson "Risks: research integrity, confidentiality, and security"](https://coderefinery.github.io/coding-with-ai/).</sup></small>
<small><sup>These slides are made using [Marp](https://marp.app/).</sup></small>

---

![Risk domains](https://coderefinery.github.io/coding-with-ai/_images/risk-domains.png)

---

![Risk domains](./assets/risks.png)

An AI writes a statistical test that runs without errors but tests the wrong hypothesis

---

![Risk domains](./assets/risks.png)

You paste an unpublished collaborator’s manuscript and analysis code into a public AI chatbot

---

![Risk domains](./assets/risks.png)

A coding agent installs a package whose name it hallucinated

---

![Risk domains](./assets/risks.png)

An agent modifies raw data files while trying to “clean up” the analysis

---

![Risk domains](./assets/risks.png)

 A prompt injection in a cloned repository makes an agent read `.env`

---

# **Research integrity**, *Confidentiality*, *Cybersecurity*
**You own the result**

--- 

The [European Code of Conduct for Research Integrity (ALLEA, revised 2023)](https://allea.org/code-of-conduct/)
rests on four principles:

| ALLEA principle | The AI-assisted coding question |
|---|---|
| **Reliability** | Does the code actually produce scientifically valid results? |
| **Honesty** | Have I transparently described how the code and result were produced? |
| **Respect** | Am I respecting participants, collaborators, licenses, and other people's work and time? |
| **Accountability** | Can I take responsibility for the code and the claims based on it? |

---

# Reliability

"The dangerous failure is not code that crashes. It is code that runs, looks reasonable, but is wrong."

Examples?
Safeguards?

---

# Honesty

Where to disclose AI use in:
- in a paper?
- in code?

---

# Respect

- other people's work
- licenses and attribution
- reviewer's time

---

# Accountability

**The AI system cannot take responsibility for your research result.**
Can you stand behind and explain:
- the analysis
- the code
- the methods
- the data transformations
- the interpretation
- the resulting claims

---

# *Research integrity*, **Confidentiality**, *Cybersecurity*
**What leaves your computer?**

---

Researchers routinely handle information that is valuable or sensitive even when it is not personal data:

- unpublished ideas, hypotheses, results, manuscripts, grant proposals;
- collaborator material, embargoed information, material under review;
- source code, proprietary algorithms, trade secrets;
- credentials, tokens, infrastructure details (server names, internal URLs);
- research-participant data, personal data, and special categories of personal data (e.g. health).

---

| Scenario | What the tool can see | Who decides |
|---|---|---|
| **Chat** | ? | ? |
| **IDE assistant** | ? | ? |
| **Agent** | ? | ? |
---
# *Research integrity*, *Confidentiality*, **Cybersecurity**
**What can the tool do?**

---

# Increasingly agentic tools can read, install, execute, modify, communicate, and authenticate
Watch out for:
- data leaving your computer (see confidentiality)
- untrusted content coming in
- wrong things installed
- insecure code written
- agents acting on systems
- over trust

---

# Risk Mitigation
**Reduce the blast radius**
- least privilege
- restrict the filesystem
- version control and backups
- review before execution
- restrict network
- use disposable, isolated environments

---

# Risks Summary: three questions

| Domain | Main question |
|---|---|
| **Research integrity** | Can I stand behind the result? |
| **Confidentiality** | What information leaves my boundary, and who can see it? |
| **Cybersecurity** | What can the tool access or do? |

---

# TU Delft

- Intranet "AI at TU Delft" https://intranet.tudelft.nl/en/group/guest/ai
- TU Delft offers Microsoft Copilot Chat through the browser
- Teaching support "AI Literacy for lecturers" https://www.tudelft.nl/teaching-support/educational-training/continuing-professional-development/ai-literacy-for-lecturers
- Help: ESA, Data Stewards, Library (https://www.tudelft.nl/research-support), Research IT Support
- TULIP is a local LLM serving platform for research and education (under development) https://tulip.pages.ewi.tudelft.nl/user-manual/