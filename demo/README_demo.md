# IKKA Demo

This folder contains public demo materials for IKKA.

IKKA is a governed AI decision infrastructure initiative for manufacturing and engineering environments.

These videos are hosted as Google Drive links and show the current product thesis, early system behavior, and demo workflows.

---

## Demo Videos

### 1. Founder Notes

A short founder video covering the broader origin story and vision behind IKKA.

[Watch Founder Notes](https://drive.google.com/file/d/1nN3HChjqATKgE-yzWrfFmknbiQqyQd0a/view?usp=sharing)

---

### 2. IKKA Intro — Terminal-Based Overview

A terminal-based walkthrough introducing the IKKA architecture, governed execution concept, and how the system is intended to process manufacturing and engineering questions.

[Watch IKKA Intro](https://drive.google.com/file/d/1kJHAAXhUQ_-OIpbjMvGXcsqDX6UQtupU/view?usp=sharing)

---

### 3. IKKA GPT — Local Evidence Retrieval

A use-case demo showing IKKA operating through a Custom GPT interface using a local evidence pack.

The demo highlights governed responses, evidence-backed reasoning, refusal behavior, and traceable outputs for manufacturing and quality-related workflows.

[Watch IKKA GPT Local Evidence Retrieval](https://drive.google.com/file/d/1eiHmfYaDOdTIPmhKdm_3I2LbRFFmtLwL/view?usp=sharing)

---

### 4. IKKA GPT — RAG Retrieval

A use-case demo showing IKKA operating through a Custom GPT interface with Onyx-backed retrieval activated.

The demo focuses on customer-specific requirement questions and shows how IKKA grounds responses in retrieved source material rather than relying on unrestricted AI generation.

[Watch IKKA GPT RAG Retrieval](https://drive.google.com/file/d/1YvUpKMLAuzdBLOE6JSYzP875bcpoCNg_/view?usp=sharing)

---

### 5. Upcoming — Controlled LLM Synthesis

A future demo will show controlled LLM synthesis once LLM capability is fully configured.

This demo will focus on how IKKA synthesizes across retrieved evidence while preserving governance constraints such as source grounding, citation integrity, traceable response paths, refusal behavior, and fallback logic.

---

## Demo Snapshot

The current public demo set includes:

* Founder vision / application video
* Terminal-based system overview
* Local Evidence Retrieval / Custom GPT use-case demo
* RAG Retrieval / Onyx-backed retrieval demo

The current demos cover two retrieval modes:

* Local evidence-pack retrieval
* Onyx-backed RAG retrieval

The next planned demo is Controlled LLM Synthesis.

## Demo KPI Snapshot

Current demo traces across Local Evidence Retrieval and Onyx RAG Retrieval:

- **Questions tested:** 14
- **Evidence Pack questions:** 10
- **Onyx RAG questions:** 4
- **Retrieval modes demonstrated:** Local evidence pack + Onyx-backed RAG
- **Out-of-domain guardrail shown:** Chocolate cake prompt rejected as outside IKKA’s governed manufacturing scope
- **Evidence-backed responses shown:** Local evidence retrieval + GM CSR retrieval
- **Local evidence files cited:** 5
- **Local evidence formats represented:** JSON, CSV, Markdown
- **Inspection records surfaced:** 135
- **GM CSR source chunks cited through Onyx:** 3
- **Onyx RAG success rate:** 4 / 4
- **Average Onyx RAG confidence:** 0.965
- **Average Onyx RAG response time:** 1.13 seconds
- **Average Onyx retrieval-backed response time:** 1.50 seconds
- **Average local evidence-backed confidence:** 1.00
- **Average local evidence-backed retrieval time:** 58.5 ms
- **Gate paths demonstrated:** Deterministic resolution, clarification, governed refusal, Gate B retrieval, Gate B / Gate C synthesis
- **Governance behaviors shown:** Out-of-domain rejection, clarification, no-evidence refusal, capability-metric withholding, compliance-certification refusal, missing-evidence disclosure
- **Work compressed:** Project context lookup, inspection review, product specification lookup, statistical summary review, launch readiness review, CSR evidence lookup, and first-pass decision framing
- **Current maturity:** MVP / pilot-development demo, not an audited production benchmark
