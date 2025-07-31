# Semantic Chain Security Model (SCSM)

**Author**: Qimin Zhao  
**Filing Date**: June 19, 2025  
**Jurisdictions**: CNIPA (China), USPTO (USA), and PCT (International)

---

## 🛡️ Patent Disclosure and Confidentiality Notice

This structural model was formally submitted as an **invention patent** to the **China National Intellectual Property Administration (CNIPA)** and the **United States Patent and Trademark Office (USPTO)**, with a simultaneous filing under the **Patent Cooperation Treaty (PCT)** on **June 19, 2025**.

> The filing date constitutes the priority date and is protected under international novelty provisions in accordance with PCT standards.

### ⚠️ Restrictions

- Any **unauthorized citation, structural replication, or standardization-based adoption** will be considered infringement.
- This content is **strictly for internal evaluation** by:
  - Recognized **standardization bodies**
  - **Qualified enterprises** under **non-public review conditions**

It is **not authorized** for:
- Public disclosure
- Reproduction
- Third-party distribution

> All conceptual content is under **active patent examination** and may **only be referenced** with **explicit written authorization**.

---

## ❓ Rethinking SOCs and the SIEM Paradigm

Modern SIEM platforms are strong in:

- Log collection
- Storage
- Indexing

But **investigation remains manual**, relying on:

- Custom rules
- Proprietary query languages (e.g., SPL, Lucene, KQL)
- Analyst experience

### Key Problems:

- **Knowledge loss** when experts leave  
- **Inconsistent log formats** across vendors  
- **High migration costs**  
- **Poor knowledge transfer**

---

## 💡 The Core Idea

> What if we replaced rule-based detection with **natural language + structured investigation paths**?

If an analyst describes a threat in plain language—  
**Could AI complete the entire investigation?**

---

## 🧠 Six Core Principles of the Model

1. **Natural language access** — lowering entry barriers  
2. **Structured behavior chains** — semantic containers  
3. **Role- and time-based modeling** — restoring context  
4. **AI semantic reasoning** — removing dependency on experience  
5. **Human-AI collaboration loops** — shared reasoning closure  
6. **Knowledge writeback mechanism** — organizational memory

---

## 🚧 Missing Layer: Investigation

Today’s platforms still center around:

> **Rules** → **Detection** → **Alerts** → **Response**

But they lack:

### 🔍 Investigation Layer

Investigation is:

- Not just log search  
- Not alert detail review  
- Not SOAR playbooks

It's the **coherent reconstruction of attacker behavior**, as humans would do.

Most platforms:

- Never define "investigation" structurally
- Rely on analysts to "figure it out"
- Offer **no native investigation capability**

---

## 📉 Consequences of the Missing Layer

- Fragmented analysis  
- Manual triage  
- Rule-centric thinking  
- Inability to form **semantic context**
- SOAR = Automation, **not** investigation

---

## 🚀 The Readiness for Change

All prerequisites are in place:

- Structured logs  
- Multisource context  
- Temporal sequencing  
- AI + NLP

Yet **investigation remains manual**—why?

> **Because we haven’t built the layer that makes investigation possible.**

---

## 🔗 Introducing: SCSM

**SCSM: Semantic Chain Security Model**

> The first system-level abstraction of **investigation** as a native platform capability—just like “detection.”

---

## 🧱 Key Concept: Behavior Chain

Instead of fragmented logs, we introduce:

> **Behavior Chain**:  
> “A sequence of actions by the same entity (user, IP, device) within a time window, grouped by chronology, context, and role consistency.”

This enables:

- Temporal reasoning  
- Intent inference  
- Risk baselining  
- False positive reduction  
- Attack path prediction

### Relation to Other Structures:

| Layer | Description |
|-------|-------------|
| **Logs** | Raw events (e.g., "User logged in at 3:00 AM") |
| **Behavior Chain** | Contextual action sequences |
| **Kill Chain** | Attack model (built upon behavior chains) |

> 📌 Kill chains are **not substitutes**, but **depend on** behavior chains.

---

## ❌ Without Behavior Chains:

- LLMs can't understand timelines  
- No behavior reasoning  
- Risk scoring fails  
- Investigation stays reactive  
- Manual log stitching continues

---

## ✅ With Behavior Chains:

- Logs = **structured sequences**  
- AI reasons on behavior, not rules  
- SOC = **semantic investigation engine**  
- Memory becomes **structured and permanent**

---

## 🧭 Implementation: SCMC Model

> SCMC (Semantic Chain Mapping Core) is the **foundation of the Investigation Layer**

- Not a rule enhancement  
- Not a SOAR plugin  
- It's a **native capability abstraction** for AI-driven investigations

---

## 🔄 Paradigm Shift

Just like:

> **Autonomous driving** redefined “driving”  
We must now:

> **Redefine investigation** in cybersecurity.

---

## 🧾 Summary

**SCSM** introduces:

- A new investigation paradigm  
- A structural fix for a long-ignored SOC gap  
- A native AI-driven reasoning layer  
- A new security architecture for the next 20 years

> **From fragmented logs → to semantic behavior chains → to AI-native investigations**

---

