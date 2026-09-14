# Business Requirements

Status: APPROVED
Owner: Namit Singh
Phase: 3 — Product Requirements
Basis: Phase 1 baseline fb5f23f; Phase 2 baseline 2f7f09d (closed 9e36d02).

> APPROVED — owner-approved as part of the Phase 3 Product Requirements baseline on 2026-09-14, after initial draft, owner CONDITIONAL PASS, amendments and final consistency review. Approval accepts this artefact as the current requirements baseline; it does NOT authorise a software build, Phase 4, or the pre-build validation gate (Phase 3.5). Prior review note: Business requirements express BUSINESS OUTCOMES, not software features. Each is traced to an approved pain point (PP), assumption (ASM), stakeholder (STK), evidence (EV) or finding (F-*). "Priority" is MoSCoW at business-outcome level and is provisional. Several outcomes could be met without dedicated software — see MVP_BOUNDARY.md. Outcomes are stated for the demonstration context (a hypothesised AI & Innovation function); they do not claim a real organisation's results.

## Reading note

An outcome being desirable does not make custom software necessary to achieve it. Where a business requirement is satisfied by the operating discipline itself (which could run on templates + existing tools), that is recorded here and challenged in MVP_BOUNDARY.md, not hidden.

---

## BR-001 — Distinguish problem from requested solution

- Requirement: The organisation must be able to separate the underlying business problem from a requested AI solution before it commits analysis or build investment.
- Rationale: Requests arrive as "Can AI solve this?"; solutioning before evidence is a hypothesised core failure mode.
- Source / evidence: PP-001, PP-002; F-A3; AS_IS_PROCESS steps 1–3.
- Related stakeholders: STK-01, STK-02, STK-03.
- Success indication: For a request, the stated problem, the requested solution and the distinction between them are recorded before options work begins.
- Assumptions / limitations: Depends on ASM-002 (BA discipline improves outcomes — OPEN).
- Priority: MUST.
- Status: APPROVED (business-outcome level).

## BR-002 — Evidence-based decisions with visible unknowns

- Requirement: The organisation must be able to base opportunity decisions on stated evidence, with unknowns visible and never converted to fact.
- Rationale: Missing baselines and asserted (not measured) value are hypothesised failure modes; AI output can hallucinate.
- Source / evidence: PP-003; F-A1; RSK-003, RSK-004.
- Related stakeholders: STK-02, STK-03, STK-05.
- Success indication: Each material claim carries an evidence reference or is explicitly marked unknown; no unknown is auto-filled.
- Assumptions / limitations: Baseline availability is ASM-006 (OPEN).
- Priority: MUST.
- Status: APPROVED.

## BR-003 — Compare AI, non-AI and no-change options

- Requirement: The organisation must be able to explicitly consider AI applicability for a request and, where AI is a credible or requested option, compare it against credible non-AI and no-change alternatives before choosing a direction; where AI is not credible or applicable, that conclusion is recorded rather than a fictional AI option being manufactured.
- Rationale: A non-AI route or "do nothing" is often the correct, defensible outcome (SCN-002); value depends on more than AI. Forcing an AI option to satisfy a template would itself be a solutioning failure.
- Source / evidence: PP-002; F-E2; SCN-002; TO-BE (LC-003).
- Related stakeholders: STK-02, STK-04, STK-01.
- Success indication: AI applicability is explicitly considered; where AI is credible, AI / non-AI / no-change options are recorded with rationale; where AI is not credible, that conclusion and the non-AI / no-change options are recorded. Non-AI and no-change remain first-class outcomes.
- Assumptions / limitations: None material beyond ASM-002.
- Priority: MUST.
- Status: APPROVED.

## BR-004 — Bring proportionate governance forward to the decision

- Requirement: The organisation must be able to capture responsible-AI/governance considerations early and obtain a specialist disposition proportionate to the opportunity's risk, before progressing the affected action.
- Rationale: Governance considered late is a hypothesised failure mode; UK governance (ICO/UK GDPR, DUAA 2025) expects DPIA triggers, ADM safeguards, oversight and fairness to be considered.
- Source / evidence: PP-005; F-D1; STK-06; ASM-007; EV-004/005/013/014.
- Related stakeholders: STK-06 (assurance authority), STK-02, STK-03.
- Success indication: Governance fields (personal-data use, DPIA trigger, ADM significance/automation level, oversight point, fairness need, accountable owner) are capturable early; a specialist disposition, including any hard blocker, is recorded before the affected action progresses. Non-legal-advice.
- Assumptions / limitations: ASM-007 (governance modelled without legal advice — OPEN). STK-06 acts as a gate depending on risk, not universally.
- Priority: MUST.
- Status: APPROVED.

## BR-005 — Define value baseline and expected-vs-actual measurement

- Requirement: The organisation must be able to define a value baseline and an expected-vs-actual measurement plan before progressing an opportunity, without fabricating ROI.
- Rationale: "Deployed ≠ adopted ≠ value"; value asserted not measured is a hypothesised failure mode.
- Source / evidence: PP-003, PP-006; F-C1/F-C2; ASM-006; EV-012 (five-layer measurement candidate).
- Related stakeholders: STK-05, STK-01, STK-08.
- Success indication: For a progressed opportunity, a baseline definition, measurement owner and expected-vs-actual plan exist; where data is unavailable this is recorded as a gap, not an invented figure.
- Assumptions / limitations: ASM-006 (baselines obtainable — OPEN); no ROI asserted.
- Priority: SHOULD (important eventual business outcome; NOT required for the pre-build validation prototype, which captures the claimed value/problem, available baseline evidence and explicit gaps only — detailed baseline + expected-vs-actual planning is deferred).
- Status: APPROVED.

## BR-006 — End-to-end traceability of the decision

- Requirement: The organisation must be able to trace any opportunity decision back to its request, evidence, assumptions, options, governance dispositions, value basis and accountable decision-makers.
- Rationale: No end-to-end traceability is a hypothesised failure mode; traceability is a candidate differentiator and a governance expectation.
- Source / evidence: PP-007; F-B2; RSK-008; RACI; TO-BE.
- Related stakeholders: STK-02, STK-06, STK-03.
- Success indication: From any decision, the full chain can be followed to its sources and owners; superseded records are retained.
- Assumptions / limitations: ASM-005 (buyers value traceability over a scoring widget — OPEN).
- Priority: MUST.
- Status: APPROVED.

## BR-007 — Transparent prioritisation separating gates from ranking

- Requirement: The organisation must be able to prioritise opportunities transparently, keeping hard gates (data/processing permission, decision-owner, funding authority, material assurance) separate from ranking inputs, so a high score cannot offset a blocker.
- Rationale: Inconsistent prioritisation is a hypothesised failure mode; a magic score that hides blockers is unsafe.
- Source / evidence: PP-004; PRIORITISATION_APPROACH; F-A2.
- Related stakeholders: STK-03 (portfolio), STK-05, STK-06.
- Success indication: Prioritisation records gate dispositions separately from ranking inputs; unresolved/blocked items are shown as such and cannot be ranked "past" a gate.
- Assumptions / limitations: Prioritisation is widely available (F-A2); differentiation is a hypothesis.
- Priority: MUST.
- Status: APPROVED.

## BR-008 — Explicit human control (AI assists; humans decide)

- Requirement: The organisation must keep human accountability explicit: AI may assist (analyse, synthesise, draft, suggest) but a human BA and the accountable authorities decide; AI output is never auto-approved.
- Rationale: Core positioning and IIBA guidance ("assistant, not authority"); AI accuracy risk.
- Source / evidence: F-B1; EV-007; DEC-002; RSK-004; BA_OPERATING_MODEL control model.
- Related stakeholders: STK-02, and all accountable authorities STK-01/03/04/05/06/07.
- Success indication: No substantive output is treated as approved without a human decision; AI-generated content is distinguishable until reviewed.
- Assumptions / limitations: None — this is a locked principle, not a hypothesis.
- Priority: MUST.
- Status: APPROVED.

## BR-009 — Proportionate outcome for every request (incl. non-AI / park / stop)

- Requirement: The organisation must be able to record a proportionate outcome for every request — including non-AI route, refine, more-evidence, park and stop — without forcing an AI solution or losing rationale.
- Rationale: A non-AI route or stop is successful BA analysis, not product failure; forcing AI is a failure mode.
- Source / evidence: SCN-002/003/004; TO-BE routes; OPPORTUNITY_LIFECYCLE (LC-006).
- Related stakeholders: STK-02, STK-03, STK-01.
- Success indication: Each request reaches a recorded disposition; park retains a revisit trigger; stop retains a reason; nothing is deleted.
- Assumptions / limitations: None material.
- Priority: MUST.
- Status: APPROVED.

## Open questions (business level)

- OQ-B1: Is the demonstration context (a single AI & Innovation function) the right unit, or should the MVP target a narrower slice (e.g. intake + evidence + governance only)?
- OQ-B2: Which of BR-001..009 genuinely require software rather than a disciplined template/process? (see MVP_BOUNDARY.md)
- OQ-B3: RESOLVED (owner) — measurement (BR-005) is SHOULD and excluded from the pre-build validation prototype; ASM-006/ASM-003 remain OPEN.
