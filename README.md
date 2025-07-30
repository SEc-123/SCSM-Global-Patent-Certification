# Semantic Chain Security Model (SCSM)

> **Patent Notice**  
This structural model was formally submitted as an invention patent application to the China National Intellectual Property Administration (CNIPA) and the United States Patent and Trademark Office (USPTO) on June 19, 2025, with a simultaneous filing under the Patent Cooperation Treaty (PCT). The application is currently under acceptance and examination. The filing date constitutes the priority date and is protected under international novelty provisions in accordance with PCT standards. Any unauthorized public citation, structural replication, or standardization-based adoption will be considered an infringement.  All conceptual content is covered under active patent examination and may not be quoted, referenced, or integrated into other systems or proposals except with explicit written authorization from the patent holder, in which case standardization is permitted.

---

## Background

Over the past few months, I have been designing and validating a system-level conceptual framework that challenges the structural logic of traditional SOC workflows and the SIEM-centric operational paradigm.

Modern SIEM platforms perform well in log collection, storage, and indexing. However, the investigation process remains heavily dependent on manual work: security analysts must write detection rules, master proprietary query languages (such as SPL, Lucene, or KQL), and examine logs line by line to reconstruct context. More critically, investigative capability relies on individual experience—when a key analyst leaves, that capability vanishes. Even worse, inconsistent log structures across different SIEM vendors lead to data fragmentation, high migration costs, and poor knowledge transferability.

---

## Core Question

So, I began thinking differently:

> What if the core of investigation were no longer about query syntax and rules, but about natural language + structured investigation paths?  
> If an analyst could describe a risk in plain language, could AI complete the entire investigation process?

---

## Six Core Principles of SCSM

This gave birth to an AI-driven security operations model built on six core principles:

1. **Natural language access** (lowering entry barriers)  
2. **Structured behavior chains** (semantic containers)  
3. **Role- and time-based behavior modeling** (context restoration)  
4. **AI semantic reasoning** (breaking reliance on experience)  
5. **Human-AI collaboration loops** (reasoning closure)  
6. **Evolving knowledge writeback mechanism** (retaining organizational memory)

---

## The Missing Architecture: The Investigation Layer

But for this model to function, a critical architectural layer must be explicitly defined — **the Investigation Layer**.

This is a foundational structure that the industry has long ignored, yet it determines whether AI can truly be integrated into security operations.

In most current platforms, the core logic still revolves around two words: **rules** and **detection**.

Rules are seen as the cornerstone of operations. They define what is “normal” and what might indicate “abnormal.” So, we build rule libraries, deploy detection systems, and set alert thresholds — everything geared toward one outcome: **triggering an alert**.

---

## Rethinking Rules

But have we asked ourselves — what is the true purpose of a rule?

- Rules are for **detection**, not for **investigation**.
- They can identify anomalies but cannot understand them.
- They can raise alarms but cannot explain what happened behind the scenes.

> **Example**: An attacker fails to log in to a server 500 times, then succeeds on the 501st attempt...

The platform has no context, no behavioral structure, and — most importantly — no **investigation layer**.  
It relies solely on rule hits, with no ability to understand behavior logic.

---

## The Structural Gap

Most platforms today are built around a familiar trio:

**Detection → Alerting → Response**

But think carefully — do any of them contain a module specifically designed for **investigation**?

Not just log search, not alert details, and not SOAR playbooks.

> I'm referring to something that can reconstruct a coherent attack story from scattered events — like a human would.

---

## Why AI Still Can’t Investigate

Today, all prerequisites for automated investigation are already in place:

- Structured logs and metadata  
- Multi-source context and time sequences  
- AI and natural language processing  

Yet **investigation remains manual** — because we haven’t built the investigation layer itself.

---

## The Semantic Chain Security Model (SCSM)

Now, I present a complete structured investigation theory: **SCSM (Semantic Chain Security Model)**.

This is not a tool to enhance rules, nor a SOAR plugin.  
It is the **first system-level abstraction of "investigation" as a native capability** — just like detection.

---

## Understanding Behavior Chains

In today’s SOC platforms, each log entry is treated as an isolated event.

> These events are either analyzed separately or loosely linked by rules —  
> but what’s missing is the **semantic structure** connecting actions and intent.

Humans understand behavior intuitively.  
AI does not.  
AI sees fragmented logs — no context, no reasoning.

The issue isn’t AI’s intelligence. The issue is the lack of structure it can reason upon.

That missing structure is the **behavior chain**.

### 📌 Definition

> “A sequence of actions performed by the same entity (user, IP, device) within a time window, aggregated by chronological order, contextual consistency, and role coherence.”

This chain can represent either normal or abnormal behavior.

---

## From Behavior Chain to Kill Chain

We define its relationship to other semantic structures as follows:

- **From logs**: raw events (e.g., “User logged in at 3:00 AM”)  
- **Behavior chain**: action sequence of a single entity  
- **Kill chain**: if the behavior chain exhibits attack intent, it can map to frameworks like MITRE ATT&CK

> ⚠️ Behavior chains are not replacements for kill chains —  
> They are the **prerequisite**.

---

## Without vs With Behavior Chains

| Without Behavior Chains | With Behavior Chains |
|-------------------------|----------------------|
| ❌ LLMs cannot understand temporal context | ✅ Logs become structured sequences |
| ❌ Behavior reasoning is impossible | ✅ Systems can model roles and deviations |
| ❌ Risk scoring lacks baselines | ✅ AI reasons based on behavior, not rules |
| ❌ Detection stays passive | ✅ SOCs evolve to semantic investigation engines |

---

## SCMC Conceptual Model

We propose a structured method to realize this vision:  
**The SCMC conceptual model as the foundation for the investigation layer.**

It is not an enhancement to existing rules.  
It is not a SOAR plugin.

> It is the **first effort to abstract investigation** as a **native platform capability** — providing the semantic map AI needs to perform investigations.

---

## Final Vision

We no longer let AI be just a **scorekeeper** — it becomes an **investigator**.  
We no longer let platforms merely **collect logs** — they become **behavior interpreters**.  
We no longer let experience **vanish** — we turn it into structured, **permanent knowledge**.

---

## Just as autonomous driving redefined what it means to "drive",  
### We are now redefining what it means to **investigate** in security operations.
