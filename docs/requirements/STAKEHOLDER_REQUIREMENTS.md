# Stakeholder Requirements

Status: APPROVED
Owner: Namit Singh
Phase: 3 — Product Requirements
Basis: STAKEHOLDER_ANALYSIS.md (STK-01..08); BA_OPERATING_MODEL; RACI; TO_BE_PROCESS.

> APPROVED — owner-approved as part of the Phase 3 Product Requirements baseline on 2026-09-14, after initial draft, owner CONDITIONAL PASS, amendments and final consistency review. Approval accepts this artefact as the current requirements baseline; it does NOT authorise a software build, Phase 4, or the pre-build validation gate (Phase 3.5). Prior review note: Stakeholder requirements state what each role legitimately needs from the operating discipline, preserving real responsibility/authority boundaries. No role is given a capability merely to simplify software. Roles are synthetic (no named individuals). Authority boundaries follow the approved RACI: the BA recommends; technical, finance, governance, operational and delivery authorities remain separate and accountable for their own dispositions.

| ID | Stakeholder | Requirement (what the role needs) | Authority boundary preserved | Source | Priority |
|---|---|---|---|---|---|
| SR-001 | STK-02 BA | Capture a request and record the distinction between stated problem and requested solution. | BA owns discovery, not spend/feasibility/governance sign-off. | BR-001; PP-001/002; BACT-001 | MUST |
| SR-002 | STK-02 BA | See unresolved evidence gaps and unknowns for an opportunity, and mark items unknown. | BA qualifies evidence; does not manufacture it. | BR-002; PP-003; BACT-002 | MUST |
| SR-003 | STK-02 BA | Explicitly consider AI applicability; where AI is credible/requested, compare AI with credible non-AI and no-change (with rationale and retained rejected options); where AI is not credible, record that conclusion rather than manufacture an AI option. | BA shortlists; technical/business owners judge usefulness/feasibility. | BR-003; SCN-002; BACT-003 | MUST |
| SR-004 | STK-01 Business requestor / operational owner | See whether and how their request is being handled, and the decision outcome with rationale; be named as decision/operational owner where applicable. | Owns the business problem and (under delegation) operational/benefit realisation; does not override specialist blockers. | BR-009; STK-01; LC-001/006 | MUST |
| SR-005 | STK-03 Head of AI & Innovation | See prioritised, evidenced opportunities with explicit blockers, to support portfolio prioritisation and go/no-go within delegated authority. | Owns portfolio priority / go-no-go within delegation; does NOT own spend/funding (that is STK-05); cannot override a hard gate by prioritising. | BR-007; PRIORITISATION; LC-005 | MUST |
| SR-006 | STK-04 Technical / Engineering | Record a feasibility/effort and data-readiness disposition for an option, with conditions. | Owns technical judgement; not asked to own business value. | BR-003/BR-004; BACT-004 | SHOULD |
| SR-007 | STK-05 Finance | See cost categories, baseline and expected-vs-actual value basis, and record a spend disposition. | Owns spend approval and benefit validation; approval to analyse ≠ approval to spend/build. | BR-005; PRIORITISATION; STK-05 | SHOULD |
| SR-008 | STK-06 Data / Privacy / Governance | See the intended data use, decision effect and automation level before giving a disposition; set conditions and hard blockers proportionate to risk. | Determines applicable assurance constraints and blockers; acts as a gate depending on risk, not universally; provides no legal advice. | BR-004; F-D1; ASM-007; BACT-004 | MUST |
| SR-009 | STK-07 Delivery / Product (receiving owner) | Receive an authorised outcome with its decision, scope, conditions, dependencies, receiving ownership and any relevant downstream requirements/acceptance material — supporting process and non-AI outcomes, not only software delivery. | Owns the receiving work once authorised; not the approver of the opportunity. | BR-006/BR-009; LC-006; RACI | SHOULD |
| SR-010 | STK-08 End user | Have adoption and real-use/outcome needs represented so value (not just deployment) can be measured. | Adopts or rejects in practice; consulted, not an approver. | BR-005; F-C1; EV-002/012 | SHOULD (LATER for live measurement) |

## Authority-boundary notes (must be preserved by any product)

- One accountable authority per bounded decision or disposition (RACI); a single opportunity may require several separate authorised dispositions (technical, privacy/governance, financial, portfolio/business) that are not collapsed. The BA (STK-02) is accountable for BA work only — proportionate discovery, evidence/options analysis, the recommendation and decision records — and NOT for technical feasibility (STK-04), data/privacy/DPIA assurance (STK-06), spend (STK-05), delivery (STK-07) or operational ownership (STK-01).
- STK-06 is a risk-proportionate assurance gate, not a universal gate on every item (STAKEHOLDER_ANALYSIS note).
- No role may progress an opportunity past an unresolved hard blocker held by the accountable specialist (BRULE-002, BRULE-003).

## Open questions (stakeholder level)

- OQ-S1: For the pre-build validation prototype, is the BA (SR-001..003) the only role that must be supported, with others satisfied by existing tools/records initially?
- OQ-S2: Should SR-010 (end-user/adoption) be explicitly LATER, given adoption measurement is post-MVP and ASM-003/ASM-004 are OPEN?
