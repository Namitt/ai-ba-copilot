# Phase 3 Synthesis and Owner Review

Status: APPROVED
Owner: Namit Singh
Phase: 3 — Product Requirements
Starting baseline: Phase 1 fb5f23f; Phase 2 content 2f7f09d; Phase 2 closure 9e36d02.

> APPROVED — owner-approved as part of the Phase 3 Product Requirements baseline on 2026-09-14, after initial draft, owner CONDITIONAL PASS, amendments and final consistency review. Approval accepts this artefact as the current requirements baseline; it does NOT authorise a software build, Phase 4, or the pre-build validation gate (Phase 3.5). Prior review note: Integrates the Phase 3 requirement set, quality review, conflict/gap analysis, product-necessity conclusion, assumption impact and open questions. PRODUCT REQUIREMENTS only — no UX, architecture, stack or code. A validation gate and Phase 4 both require separate owner authorisation; neither is executed or assumed here.

## Executive finding

An implementation-neutral requirement set (9 BR, 10 SR, 32 FR, 11 NFR, 12 BRULE, 12 US, 28 AC) is derived cleanly and traceably from the approved Phase 1 discovery and Phase 2 operating-model baselines, preserving the control model (AI assists; humans decide) and the non-negotiable safety controls. **Deriving requirements does not establish that a dedicated application is necessary.** The requirement set now separates a **PRE-BUILD VALIDATION PROTOTYPE** (templates + existing tools; tests ASM-002/ASM-004) from a **CONDITIONAL SOFTWARE MVP** (only if a validation gate and owner decision justify it). The product-necessity challenge — reassessed conservatively (custom product vs configurable existing tool) — finds **no capability proven to require a custom build**; the strongest, still-unproven, case is an integrated enforced-control-plus-traceability layer. ASM-002, ASM-004 and ASM-010 remain OPEN; the product hypothesis remains PARTIALLY SUPPORTED / REQUIRES FURTHER VALIDATION.

## Requirement set summary

| Type | Count | Notes |
|---|---|---|
| Business Requirements (BR) | 9 | Outcomes; BR-005 (measurement) is SHOULD, not in the validation prototype |
| Stakeholder Requirements (SR) | 10 | Authority boundaries preserved (STK-03 no spend; SR-009 supports non-software handoff) |
| Functional Requirements (FR) | 32 | Implementation-neutral; AI/DET/HUMAN classified; FR-026..029 CONDITIONAL MUST — IF AI ENABLED |
| Non-Functional (NFR) | 11 | No fabricated numbers; NFR-002 conditional on AI; NFR-010 CANDIDATE/unsupported |
| Business Rules (BRULE) | 12 | Govern the process; BRULE-011 = one authority per bounded decision/disposition |
| User Stories (US) | 12 | Behavioural catalogue; not all MUST; US-004/US-010 conditional/SHOULD |
| Acceptance Criteria (AC) | 28 | Observable; measurement AC (023/024) conditional on measurement being in the next action |

## Requirements quality review (honest)

| Flag | Items | Note |
|---|---|---|
| Ambiguous | none blocking | "proportionate"/"material" are deliberate human-judgement terms from the approved baseline |
| Conflicting | see conflict analysis | trade-offs recorded, not resolved by assuming the product wins |
| Unsupported (no approved source) | **NFR-010 (accessibility)** | deliberately retained as a CANDIDATE with NO TRACEABLE JUSTIFICATION; not MUST, not falsely sourced |
| Duplicate | none | FR groups distinct; overlaps are layer relationships |
| Solution-biased | FR-003, FR-009, FR-014 | flagged NEEDS VALIDATION; not MUST |
| Not fully testable yet | NFR-010, NFR-011 | ACs are observable, but NFR-010 has no applicable target set and NFR-011's acceptance approach is still to be defined before build — recorded as pending, not claimed testable |
| Needs owner decision | OQ list below | scope, necessity, validation-gate questions |

We do **not** claim "Unsupported: none" — NFR-010 is honestly retained without approved evidence.

## Conflict / gap analysis (unresolved — for owner)

| Tension | Nature | Not resolved by |
|---|---|---|
| Governance/control vs speed | hard gates + traceability add friction (NFR-007) | assuming users tolerate it — ASM-004 OPEN |
| Traceability vs workflow burden | more recording may reduce adoption (RSK-009) | assuming the product wins; NFR-007 to validate |
| AI assistance vs deterministic control | AI speed vs provenance overhead | including AI in the prototype — kept out; AI controls conditional |
| Standardised process vs proportionality | one model vs proportionate depth | forcing every request through all stages (TO-BE allows abbreviation) |
| Custom product vs configurable existing tool | build vs configure Jira/Notion | assuming a build is needed — necessity unproven |
| Portfolio comparison vs incomparable evidence | ranking dissimilar opportunities | a single score — gates kept separate from ranking |

Gaps: no real-user evidence (all synthetic); measurement feasibility unproven (ASM-006); market gap documentation-based only (RSK-001).

## Product-necessity conclusion (mandatory)

1. **Which capabilities actually require a custom product?** On current evidence, **none is proven to require it.** Templates and configurable existing tools (Jira/Notion, forms, spreadsheets) plausibly cover the validation prototype and possibly more, including *some* hard-gate enforcement, permissions and traceability.
2. **Which could live in existing tools/process?** Intake/framing, evidence-with-unknowns, options (incl. non-AI), governance capture, transparent prioritisation, and much traceability/permissioning.
3. **Strongest justification for AI BA Copilot as a dedicated product?** A still-unproven hypothesis of *integration value*: one coherent operating control layer combining enforced control discipline, authority separation, provenance, traceability and controlled reopen/change — hard to assemble reliably from configured tools. Not proven necessary.
4. **Evidence still needed before build investment?** Real-user validation of ASM-002 and ASM-004; hands-on evaluation of comparable tools AND of configuring an existing tool to the discipline (RSK-001/ASM-005); measurement feasibility (ASM-006); evidence on ASM-010.

## Recommended owner decision (not executed; roadmap not rewritten as approved)

Consider inserting a **validation gate between Phase 3 and Phase 4**: a no-code discipline prototype (templates + Jira/Notion) to test ASM-002/ASM-004, and a head-to-head look at configuring an existing tool, before committing to any build. This is a recommendation for the owner to decide at final Phase 3 review — it is **not** authorised, not started, and does not pre-approve Phase 4 or a build.

## Assumption impact

| Assumption | Status | Change | Evidence |
|---|---|---|---|
| ASM-002 (BA discipline improves outcomes) | OPEN | unchanged | primary target of a future validation prototype; not validated |
| ASM-004 (adoption/burden) | OPEN | unchanged | primary target of a future validation prototype; NFR-007 makes it testable |
| ASM-010 (intake drives value gap) | OPEN | unchanged | NOT testable by a small process pilot; needs comparative/longitudinal real-world evidence |
| ASM-005 (buyers value traceability over scoring) | OPEN | unchanged | product value narrowed to integrated control/traceability; still to test |
| ASM-006 (baselines obtainable) | OPEN | unchanged | measurement kept SHOULD; excluded from the prototype |
| ASM-003/007/008/009 | OPEN | unchanged | — |
| ASM-001 (value gap) | VALIDATED (secondary) | unchanged | not re-litigated |

No assumption is promoted because Phase 3 produced requirements.

## What remains unproven

Enterprise causation, real-user adoption, measurable net benefit, market differentiation, buyer preference and technical feasibility remain unproven. A traceable requirement set does not establish that a dedicated application is necessary, nor that the concept is differentiated. Phase 4 (UX/IA), Phase 5 (Architecture/Data) and Phase 6 (AI/Tool evaluation) have not begun.

## Open questions for the owner

- OQ-1 — **APPROVED** (owner): requirement hierarchy and the validation-prototype vs software-MVP distinction accepted.
- OQ-2 — **OPEN**: whether to authorise a validation gate / Phase 3.5 (no-code prototype) between Phase 3 and Phase 4 to test ASM-002/004 before any build. Recommended; NOT authorised — the next owner roadmap decision.
- OQ-3 — **ACCEPTED** (owner): no capability is proven to require a custom product; the integrated control + authority-separation + provenance + traceability + controlled-change layer remains the strongest, still-unproven, custom-product hypothesis.
- OQ-4 — **OPEN**: whether the validation gate should include a configured-existing-tool evaluation head-to-head with a custom product before any build decision. NOT authorised.
- OQ-5 — **RESOLVED** (owner): no further Phase 3 requirement reclassification required at closure.
- OQ-6 — **RESOLVED** (owner): measurement (BR-005) remains SHOULD and outside the pre-build validation prototype (ASM-006 OPEN).
- OQ-7 — **RESOLVED** (owner): Request and Opportunity Case are distinct concepts, initially one-to-one.
- OQ-8 — **RESOLVED** (owner): no INFO identifier family in Phase 3; information items stay conceptual/unnumbered.

## Verification scope (for this phase)

Confirm: BRs are outcomes not features; SRs preserve authority (STK-03 ≠ spend; SR-009 supports non-software handoff); FRs implementation-neutral; NFRs free of fabricated numbers and honest about NFR-010; BRULEs separated from implementation (BRULE-011 = one authority per bounded decision/disposition); AI/DET/HUMAN explicit; AI cannot approve; unknown cannot become fact; human review explicit; non-AI/park/stop valid; no fictional AI option; requirements proportionate (no screen-per-stage); measurement not mandatory in the prototype; AI controls conditional on AI; ASM-002/004/010 OPEN; ASM-010 not claimed testable by a small pilot; product necessity still challenged (custom vs configurable); validation prototype ≠ software MVP; no architecture/UI/stack/provider/code; repo uncommitted/unpushed. No software test suite applies — no software changed.
