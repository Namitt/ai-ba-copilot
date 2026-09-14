# Product Scope and Requirement Hierarchy

Status: APPROVED
Owner: Namit Singh
Phase: 3 — Product Requirements
Basis: Phase 1 discovery baseline fb5f23f; Phase 2 operating-model baseline 2f7f09d (closed 9e36d02).

> APPROVED — owner-approved as part of the Phase 3 Product Requirements baseline on 2026-09-14, after initial draft, owner CONDITIONAL PASS, amendments and final consistency review. Approval accepts this artefact as the current requirements baseline; it does NOT authorise a software build, Phase 4, or the pre-build validation gate (Phase 3.5). Prior review note: Implementation-neutral product requirements only — no UX, architecture, stack, data model or code. Phase 4 (UX/IA), Phase 5 (Architecture/Data) and Phase 6 (AI/Tool evaluation) come later. The approved Phase 2 conclusion stands: the six-stage operating model is internally coherent across synthetic stress tests, but this does NOT establish that a dedicated software application is necessary. ASM-002, ASM-004 and ASM-010 remain OPEN; the product hypothesis is PARTIALLY SUPPORTED / REQUIRES FURTHER VALIDATION.

## 1. Purpose

Define the product boundary and requirement hierarchy for AI BA Copilot before any detailed requirement, so that every requirement is derived from an approved business/decision need — not from mechanically turning each operating-model stage into a screen or feature.

## 2. Product intent (from the approved baseline)

AI BA Copilot is a BA-led operating discipline for turning an unstructured business request into an evidenced, prioritised, governed and measurable AI (or non-AI) opportunity decision, with AI assisting and a human BA and accountable authorities deciding (PRODUCT_VISION, BA_OPERATING_MODEL). Phase 3 asks: **which of that discipline genuinely needs dedicated software, and what would the requirements be if it did?**

## 3. Core business concepts

- **Request** — the original stakeholder ask / source input.
- **Opportunity case** — the governed analysis record used to evaluate whether and how a request should progress.

Initial model: one opportunity case per request unless later validation shows a need for split/merge (see INFORMATION_REQUIREMENTS.md). "Opportunity" below means the opportunity case.

## 4. Requirement hierarchy

```
Business need / approved evidence (PP-###, ASM-###, EV-###, findings F-*)
        ↓
BR-###   Business Requirement        (business outcome)
        ↓
SR-###   Stakeholder Requirement     (what a role needs)
        ↓
FR-### / NFR-### / BRULE-###         (product capability / quality / governing rule)
        ↓
US-###   User Story
        ↓
AC-###   Acceptance Criterion
```

Not every BR spawns every downstream type. Traceability reflects real dependency, not one-to-one mapping. Identifier families are the existing ones registered in `docs/governance/IDENTIFIER_STANDARD.md` (BR, SR, FR, NFR, BRULE, US, AC); none are renumbered. **Conceptual information needs are listed unnumbered in INFORMATION_REQUIREMENTS.md; no INFO identifier family is added in Phase 3.**

## 5. Two distinct concepts: validation prototype vs software MVP

The single most important scope point (owner review): "MVP" was previously used for two different things. They are now separated.

### 5.1 PRE-BUILD VALIDATION PROTOTYPE
- **Purpose:** test the BA operating discipline itself **before any build commitment**.
- **Potential form:** structured templates + Jira/Notion/Excel (or equivalent existing tools). **Not** a dedicated application; do not call it an application MVP.
- **Primary assumptions tested:** **ASM-002** (does the structured BA discipline improve decision quality/consistency?) and **ASM-004** (can/will intended practitioners use the discipline without disproportionate burden?).
- **Not tested:** ASM-010 (enterprise causation — needs comparative/longitudinal real-world evidence; stays OPEN). The prototype may generate useful observations about intake quality but must not claim to validate enterprise causation.
- **Status:** a **recommended validation gate for owner decision** — NOT authorised for execution here, and not started.

### 5.2 CONDITIONAL SOFTWARE MVP
- Only relevant **if** the validation gate and a subsequent owner decision justify custom software.
- Should focus on capabilities where dedicated software may **materially improve control, enforcement, traceability or provenance** (see MVP_BOUNDARY.md product-necessity taxonomy).
- Whether it is needed at all is UNPROVEN (product-necessity challenge).

## 6. Capability scope (applies to the discipline; where each lands is decided later)

### 6.1 Core discipline capabilities (candidate MUST for the validation prototype)
- Capture a request and separate stated problem from requested solution (BR-001).
- Record evidence with explicit unknowns; prevent unknown becoming fact (BR-002).
- Explicitly consider AI applicability; where AI is credible, compare AI / non-AI / no-change (no fictional AI option) (BR-003).
- Capture proportionate responsible-AI/governance fields early and record a specialist disposition, incl. hard blockers (BR-004).
- Maintain end-to-end traceability of the decision chain (BR-006).
- Transparent prioritisation separating hard gates from ranking inputs (BR-007).
- Explicit human control: AI assists, humans decide; AI output marked unreviewed **when AI is used** (BR-008).
- Record a proportionate outcome incl. non-AI route / park / stop (BR-009).
- Capture the claimed value/problem, available baseline evidence and explicit uncertainty/gaps (BR-002). **Detailed value-baseline + expected-vs-actual measurement planning (BR-005) is SHOULD — NOT required for the pre-build validation prototype.**

### 6.2 LATER — post-validation / post-MVP
- Pilot execution and live adoption/outcome measurement; portfolio dashboards; integrations; automated evidence collection; multi-team scale.

### 6.3 OUT OF SCOPE (this and adjacent phases)
- UX/screen/wireframe design (Phase 4); architecture, data model, API, hosting (Phase 5); AI provider/model, embeddings/vector store, agent framework, RAG stack (Phase 6); application code, infrastructure, developer tasks/sprints; any real-company or real-personal data; any legal advice; autonomous AI decision-making; fabricated performance/SLA/security numbers or invented user research.

### 6.4 NEEDS VALIDATION before commitment
- Whether a dedicated application (vs templates + existing tools vs a configurable existing tool) is necessary (MVP_BOUNDARY.md).
- ASM-002 (discipline improves outcomes), ASM-004 (adoption/burden), ASM-006 (baselines obtainable), ASM-010 (intake drives value gap), RSK-001 (market gap).

## 7. What Phase 3 deliberately does not resolve

Phase 3 does not resolve the application-necessity question and must not resolve it by assumption. It produces requirements conditional on that question, an explicit product-necessity challenge (MVP_BOUNDARY.md), and a recommended validation gate for owner decision (PHASE3_SYNTHESIS.md). The roadmap is not rewritten as though a validation exercise or a build were already approved.

## 8. Artefact set (all DRAFT, this phase)

PRODUCT_SCOPE.md (this) · BUSINESS_REQUIREMENTS.md · STAKEHOLDER_REQUIREMENTS.md · FUNCTIONAL_REQUIREMENTS.md · BUSINESS_RULES.md · INFORMATION_REQUIREMENTS.md · NON_FUNCTIONAL_REQUIREMENTS.md · USER_STORIES_AND_AC.md · TRACEABILITY_MATRIX.md · MVP_BOUNDARY.md · PHASE3_SYNTHESIS.md. All under `docs/requirements/`; GitHub is the detailed version-controlled authority.
