# How IKKA Works

## High-Level Architecture

IKKA is a governed AI infrastructure layer for manufacturing and engineering environments where AI-assisted responses need to be evidence-aware, traceable, and controlled.

The current MVP follows a modular architecture:

| Layer                                 | Role                                                                                   |
| ------------------------------------- | -------------------------------------------------------------------------------------- |
| User / Workflow Interface             | Entry point for manufacturing, quality, engineering, or business users                 |
| IKKA API Layer                        | Receives requests and returns structured responses                                     |
| Governance + Routing Layer            | Determines the appropriate response path                                               |
| Context / Retrieval / Synthesis Layer | Uses structured context, approved evidence, and controlled synthesis where appropriate |
| Structured Response + Trace           | Returns an answer with confidence, risk, citations, and trace metadata                 |

IKKA is not designed to treat every request as an open-ended AI prompt. The system is built to determine the appropriate response path before producing an answer.

---

## Current Runtime Stack

The current IKKA MVP uses a lightweight, modular architecture.

Current components include:

* local application code
* FastAPI-based API service
* Docker-based runtime environment
* Cloudflare tunnel / domain access for external demo workflows
* Onyx-backed retrieval for RAG workflows
* Onyx / LLM-backed synthesis where enabled
* local evidence-pack mode for controlled demo and fallback scenarios
* structured response objects with citations, confidence, risk-band, and trace fields

This stack is being used for MVP validation, demo workflows, and pilot-readiness testing.

The architecture is designed to remain model- and provider-flexible over time.

---

## Knowledge and Evidence Sources

IKKA is designed to work with approved knowledge sources rather than relying only on open-ended model generation.

Current evidence handling includes:

* structured project context staged through JSON
* product and program information staged through controlled local files
* meeting notes and workflow context staged as public-safe demo records
* inspection data staged through CSV and statistical summary files
* document and standards retrieval supported through RAG connectors
* customer-specific requirements and quality references supported through approved retrieval sources where available

In the public demo environment, IKKA uses sanitized or public-safe materials only.

Customer-specific data, private evidence packs, proprietary documents, internal prompts, scoring logic, and production deployment details are not included in this repository.

---

## Response Behavior

IKKA responses are designed to support manufacturing and engineering decision workflows.

A structured response may include:

* answer
* citations or source references
* confidence signal
* risk band
* trace information
* clarification or refusal message where applicable

The purpose is to make AI-assisted responses easier to review, validate, and improve over time.

---
