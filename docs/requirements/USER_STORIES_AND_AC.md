# User Stories and Acceptance Criteria

Status: APPROVED
Owner: Namit Singh
Phase: 3 — Product Requirements
Basis: STAKEHOLDER_REQUIREMENTS (SR); FUNCTIONAL_REQUIREMENTS (FR); BUSINESS_RULES (BRULE).

> APPROVED — owner-approved as part of the Phase 3 Product Requirements baseline on 2026-09-14, after initial draft, owner CONDITIONAL PASS, amendments and final consistency review. Approval accepts this artefact as the current requirements baseline; it does NOT authorise a software build, Phase 4, or the pre-build validation gate (Phase 3.5). Prior review note: Stories express user intent, not screen design. Acceptance criteria are observable, testable and implementation-neutral (Given/When/Then where it adds precision). These are NOT full UAT scripts (detailed UAT is a later phase). Control criteria (unknown stays unknown; AI output distinguishable until reviewed; blocked cannot progress; non-AI route valid; PARK/STOP retain rationale; authority respected) are included where the story touches them.

---

## US-001 — Capture a request without solutioning
As a **Business Analyst (STK-02)**, I want to record a request with its stated problem separate from its requested solution, so that analysis starts from the problem, not the tool.
Traces: SR-001, FR-001/002; BR-001.
- AC-001: Given a new request, when it is recorded, then "stated problem" and "requested solution" are stored as distinct fields.
- AC-002: Given options work is marked complete while the problem/solution distinction is unrecorded, then the product flags it as incomplete.

## US-002 — See what is unknown
As a **BA (STK-02)**, I want unknowns to stay visibly unknown, so that gaps are not mistaken for facts.
Traces: SR-002, FR-004/005/006; BRULE-005.
- AC-003: Given a field with no evidence, when the opportunity is viewed, then the field shows "unknown" and is not auto-populated.
- AC-004: Given an AI-suggested value, then it is visibly distinct from a human-confirmed value until a human confirms it.
- AC-005: Given unresolved evidence gaps, then they are listed for the BA.

## US-003 — Compare AI, non-AI and no-change
As a **BA (STK-02)**, I want to explicitly consider AI applicability and, where AI is credible, compare AI with non-AI and no-change (recording the conclusion where AI is not credible), so that a non-AI route or "do nothing" is a first-class outcome and no fictional AI option is created.
Traces: SR-003, FR-007/008; BR-003; SCN-002.
- AC-006: Given a request, when options are recorded, then AI applicability is explicitly considered; where AI is credible, AI / non-AI / no-change options exist with rationale; where AI is not credible, that conclusion is recorded with the non-AI / no-change options (no fictional AI option).
- AC-007: Given a rejected option, then it is retained with its reason.
- AC-008: Given the analysis concludes non-AI is preferable, then "non-AI route" is a valid recorded outcome.

## US-004 — Use AI assistance under control (CONDITIONAL — only if AI assistance is included; not required for the pre-build validation prototype)
As a **BA (STK-02)**, I want AI to draft summaries and candidate options from my source material, so that I work faster — while I stay the decider.
Traces: FR-003/009/026/027/028/029; BR-008; BRULE-004.
- AC-009: Given AI produces content, then it is marked AI-generated and "unreviewed" until a human reviews it.
- AC-010: Given an AI summary, then it preserves links to the source material.
- AC-011: Given the AI capability is unavailable or rate-limited, then the workflow continues and the BA can proceed manually.
- AC-012: Given AI output, when a human edits or rejects it, then the change is retained; AI output is never treated as an approval.

## US-005 — Capture governance early
As a **Governance specialist (STK-06)**, I want to see intended data use, decision effect and automation level before I give a disposition, so that assurance is informed, not a late blocker.
Traces: SR-008, FR-010/011; BR-004; F-D1.
- AC-013: Given an opportunity, then governance fields (personal-data use, DPIA trigger, ADM significance/automation level, oversight point, fairness need, accountable owner) are capturable early.
- AC-014: Given a specialist reviews an option, then they can record a disposition of passed / conditions / blocked, with conditions and scope.

## US-006 — Blocked cannot progress
As an **accountable authority**, I want a hard blocker to stop the affected action, so that value cannot override assurance.
Traces: FR-012/018; BRULE-002/003.
- AC-015: Given an unresolved hard blocker on an action, when progression is attempted, then it is prevented until the blocker is cleared by the accountable specialist.
- AC-016: Given a high value/ranking, then it does not allow the action to pass an unresolved hard gate.

## US-007 — Early referral returns to discovery
As a **BA (STK-02)**, I want an early governance referral to return to discovery/options, so that problem understanding and options are not skipped.
Traces: FR-013; BRULE-007; TO-BE routing.
- AC-017: Given an early triage referral, when it resolves as safe to continue, then the opportunity returns to discovery (LC-002), not to LC-004 assurance.
- AC-018: Given a held activity, then safe desk analysis / alternative-option exploration can continue while it is held, only within the scope and conditions allowed by the relevant specialist disposition.

## US-008 — Prioritise transparently
As a **Head of AI & Innovation (STK-03)**, I want to see prioritised, evidenced opportunities with explicit blockers, so that portfolio prioritisation, recommendation and go/no-go within my delegated authority are defensible (spend/funding authority remains with Finance, STK-05).
Traces: SR-005, FR-017/019; BR-007.
- AC-019: Given a set of eligible opportunities, then hard-gate dispositions are shown separately from ranking inputs.
- AC-020: Given a BA recommendation, then it is marked a recommendation (not an approval) and carries alternative, conditions, confidence and a reconsideration trigger.

## US-009 — Record the decision and handoff
As an **accountable authority**, I want to record the decision with rationale, conditions and owners, so that the outcome is traceable and the receiving owner is clear.
Traces: SR-004/009, FR-020/021/022/025; BR-009; LC-006.
- AC-021: Given a decision, then it records one accountable authority, rationale, conditions, dissent (if any), reviewer and date.
- AC-022: Given a park, then a revisit trigger is retained; given a stop, then a reason is retained; neither deletes the record.
- AC-023: Given a proceed decision, then a receiving owner is recorded; where value measurement is part of the authorised next action, a measurement owner is recorded; otherwise the measurement gap/condition is preserved explicitly (not universally required).

## US-010 — Define how value will be measured (SHOULD / conditional — detailed measurement is not required for the pre-build validation prototype)
As **Finance (STK-05)**, I want a baseline and expected-vs-actual measurement plan, so that value is measured, not asserted.
Traces: SR-007, FR-014/015/016; BR-005.
- AC-024: Given value measurement is part of the decision / authorised next action, then a baseline, measurement owner and expected-vs-actual plan exist, or the gap is recorded (no invented figure).
- AC-025: Given released capacity, then it is not stated as cash saving without a supported basis, and no ROI is asserted where costs are unknown.

## US-011 — Follow the trace
As a **BA / auditor (STK-02/06)**, I want to follow any decision back to its evidence and owners, so that the decision is defensible.
Traces: FR-023/024/031; BR-006.
- AC-026: Given a decision, then the chain back to request, evidence, assumptions, options, assurance, value basis and authorities is navigable.
- AC-027: Given a material change to purpose/data/decision-effect/cost/ownership, then the relevant gate reopens and superseded records are retained.

## US-012 — Respect who may act
As the **owner**, I want only the legitimately authorised role to take each action, so that authority separation holds.
Traces: FR-032; BRULE-011; NFR-003.
- AC-028: Given an assurance disposition, then only the accountable specialist can record it; given a spend disposition, then only the funding authority can record it; given a decision, then only the accountable authority can record it.

## Note on scope

The story catalogue covers the Phase 3 behavioural requirements, **including conditional/SHOULD stories** (e.g. US-004 AI-assist, US-010 measurement). Inclusion in this catalogue does NOT mean inclusion in the pre-build validation prototype or a later software MVP — that is decided in MVP_BOUNDARY.md. Not all stories are MUST.

## Open questions (story level)

- OQ-U1: RESOLVED (owner) — US-004 (AI assistance) is excluded from the pre-build validation prototype, isolating whether the discipline (not the AI) drives any improvement (ASM-002).
- OQ-U2: RESOLVED (owner) — US-010 (measurement) is SHOULD and not in the pre-build validation prototype (ASM-006 OPEN).
