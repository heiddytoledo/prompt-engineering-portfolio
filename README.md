# Prompt Engineering Portfolio
### Heiddy Toledo · WakIA · Tulsa, Oklahoma

---

## About This Repository

I'm a prompt engineer and curriculum designer specializing in AI systems for education and business automation. This repository documents the technical architecture behind **FORMALIZA** — a 28-day AI-tutored program that guides Spanish-speaking entrepreneurs through the legal and tax formalization of their U.S. businesses.

FORMALIZA is not a prototype. It is a certified, live educational product:
- Certified by **Florida Global University** (institution #10191)
- AI tutor built on **Claude API by Anthropic**
- Platform live at [wakia.app](https://wakia.app)

---

## What You'll Find Here

### `/FORMALIZA` — Prompt Engineering System

The complete prompt architecture behind **Próspero**, the AI tutor that guides students through 28 days of curriculum.

| File | What it shows |
|---|---|
| `00_SYSTEM_PROMPT_MAESTRO.md` | Master system prompt — identity, guardrails, conditional routing, 5-phase daily flow |
| `01_DOC-ID-01_Identidad.md` | Agent identity design — personality, tone states, failure mode handling |
| `03_DOC-OP-01_Flujo_Diario.md` | Operational protocol — daily 5-phase interaction structure, deliverable evaluation |

### `FORMALIZA_CaseStudy_HeidyToledo.docx`

A detailed case study (in English) documenting:
- The 3-layer prompt architecture (system prompt + RAG + dynamic context)
- Conditional user-path design for 3 distinct user profiles
- Safety guardrails for regulated content (legal and tax domain)
- Socratic tutoring method implemented in natural language instructions
- Honest reflection on what I would do differently

---

## Core Technical Decisions

**Why a 3-layer architecture instead of 28 individual prompts:**
A single master system prompt + knowledge base + minimal daily context injection reduces token costs, eliminates instruction contradictions across days, and makes the system maintainable when IRS rates update annually.

**Why conditional routing in natural language:**
Three user profiles (physical U.S. business / digital U.S. business / outside U.S.) require completely different guidance on legal structure, state registration, and tax obligations. This routing is implemented as explicit conditional instructions in the system prompt — the model handles routing, I handle the rules.

**Why explicit guardrails matter in regulated domains:**
Legal and tax content carries real financial risk to users. Próspero explains concepts and shows options — it never gives specific legal advice for individual situations. Every topic with legal implications has a mandatory escalation instruction and a standard disclaimer embedded in the system prompt.

---

## Skills Demonstrated

- Multi-layer prompt architecture design
- Conditional instruction logic (without code)
- Safety guardrail design for regulated content domains
- Pedagogical AI design (Socratic method, deliverable evaluation, escalation logic)
- Complexity reduction: IRS tax code → accessible decision trees
- Knowledge base structure for RAG-based tutoring systems
- Pipeline design: 28-day chained instructional context

---

## Background

I come from digital journalism — my core competencies are research, verification, and making complex information accessible to non-expert audiences. Applied to AI, that means: designing systems that give accurate, safe, and understandable outputs to people who can't afford to get it wrong.

FORMALIZA was built without writing a single line of code. The architecture is in the prompts.

---

## Contact

**Heiddy Toledo**  
Founder, WakIA  
heiddy@wakia.app  
[wakia.app](https://wakia.app) · Tulsa, Oklahoma
