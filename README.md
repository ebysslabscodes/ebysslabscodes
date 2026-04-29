# RISWIS

Control what your AI is allowed to use — before it generates anything.

**Governance Layer for AI Systems**

A control layer that sits between retrieval and generation — deciding what data the model is allowed to use before anything is generated.

Live system with real ranking and decision logic.

---

### The Problem

Most AI systems follow this pattern:

**Retrieve → Send to model → Generate**

There is no control over what actually reaches the model.

Low-quality, outdated, or untrusted sources are treated the same as authoritative ones.

The result:
- unreliable outputs
- no visibility into why something was used
- no enforceable trust boundary

---

### The RISWIS Approach

RISWIS changes the order:

**Retrieve → Govern → Generate**

It enforces explicit policy decisions on retrieved data before it reaches the LLM.

---

### What RISWIS Does

- Re-ranks results using defined trust tiers (T1 / T2 / T3)
- Separates **semantic ranking from policy decisions**
- Surfaces **semantic winner vs policy winner**
- Detects rank flips and overrides
- Makes enforceable decisions: **ALLOW / REVIEW / BLOCK**
- Returns auditable outputs with scores, multipliers, and flags
- Prevents untrusted data from reaching the model

---

### Core Principle

Similarity finds answers.  
**Governance decides what gets used.**

semantic winner ≠ policy winner

---

### Who It's For

- AI startups building production RAG systems
- Teams shipping customer-facing or internal AI tools
- Companies in regulated environments (healthcare, finance, legal)
- Anyone responsible for what their AI outputs

---

### Live Demo

→ https://riswis.com

Interactive demo of the decision layer.

---

### Current Status

- Working prototype with live ranking + decision logic
- API endpoints: `/rank` and `/decide`
- Actively moving toward production deployment

---

### Other Work

**CAS 2.0** — Long-horizon evaluation framework for system drift and stability.

---

### Contact

X: https://x.com/ebysslabs  
GitHub: https://github.com/ebysslabscodes  
Email: ronreed@ebysslabs.com

---

Built by **Ronald Reed (Ebysslabs)**
