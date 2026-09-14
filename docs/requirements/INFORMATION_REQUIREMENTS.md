# Information Requirements (Conceptual)

Status: APPROVED
Owner: Namit Singh
Phase: 3 — Product Requirements
Basis: OPPORTUNITY_LIFECYCLE; TO_BE_PROCESS; BA_OPERATING_MODEL; PRIORITISATION_APPROACH.

> APPROVED — owner-approved as part of the Phase 3 Product Requirements baseline on 2026-09-14, after initial draft, owner CONDITIONAL PASS, amendments and final consistency review. Approval accepts this artefact as the current requirements baseline; it does NOT authorise a software build, Phase 4, or the pre-build validation gate (Phase 3.5). Prior review note: This lists the BUSINESS INFORMATION that must exist to support the operating process. It is conceptual only — NOT a database schema, table structure, entity-relationship model or API payload. Phase 5 (Architecture / Data) designs the data model. Items are grouped by the lifecycle stage that first needs them; an item may be read or updated at later stages.

## Core business concepts (implementation-neutral)

Two business concepts are defined now (the *meaning*, not a data model — Phase 5 designs any tables/relationships):

- **Request** — the original stakeholder ask / source input ("Can AI solve this?") as received via meeting, message, idea or complaint.
- **Opportunity case** — the governed analysis record used to evaluate whether and how a request should progress (it carries problem/solution, evidence, options, governance, value basis, decision and traceability).

For MVP simplicity the initial model assumes **one opportunity case per request**, unless later validation demonstrates a genuine need for split (one request → several cases) or merge (several requests → one case) behaviour. This resolves OQ-I1: request and opportunity case are distinct concepts, related one-to-one for now. Elsewhere in the requirement set, "opportunity" means the opportunity case.

## Information needs by lifecycle stage

| Stage | Information that must exist | Notes |
|---|---|---|
| LC-001 Triage | Opportunity/request identity; source/channel; stated problem; requested solution; intended decision/use; business/operational owner; sensitivity/urgency flags; initial risk flags | "Stated problem" and "requested solution" are distinct items (BRULE-001, FR-002). |
| LC-002 Evidence | Current-process description; baseline definition/period/denominator; evidence references; assumptions; competing-cause notes; explicit unknowns/gaps | Unknown is a first-class value (BRULE-005). |
| LC-003 Options | Option set with explicit AI-applicability consideration (AI where credible, else the recorded conclusion; non-AI; no-change); per-option rationale; retained rejected options with reasons; potential harms | Rejected options retained (BRULE-010); no fictional AI option (BR-003/FR-007). |
| LC-004 Assurance | Governance fields: personal-data use; DPIA trigger; ADM significance/automation level; oversight point; fairness/transparency need; accountable owner. Per-option assurance disposition (passed/conditions/blocked); conditions; scope; re-review trigger; feasibility/data-readiness disposition | Non-legal-advice; specialist owns the disposition (SR-008). |
| LC-004/005 Value | Claimed value/problem; available baseline evidence; explicit uncertainty/gaps (always). Detailed value information — baseline definition/period, cost categories, measurement owner, expected value range, expected-vs-actual plan — is CONDITIONAL: required only where value measurement is part of the authorised next action (BR-005 is SHOULD); otherwise the gap/condition is preserved. | "Released capacity" separate from "cash saving" (FR-016); no invented figures. |
| LC-005 Prioritisation | Hard-gate dispositions (permission, decision-owner, funding authority, assurance) separate from ranking inputs; confidence; trade-offs; dependencies | Gates separate from ranking (BRULE-003). |
| LC-006 Decision | Decision (proceed/non-AI/refine/more-evidence/park/stop); rationale; conditions; accountable authority; dissent; reviewer/date; receiving owner (where applicable); measurement owner ONLY where value measurement is part of the authorised next action (otherwise the measurement gap/condition is preserved); revisit/reopen trigger; superseded records | Retention and reopen rules (BRULE-006/008/010); measurement conditional (FR-022/AC-023). |
| Cross-cutting | Traceability links across the chain; record status (unknown / human-confirmed / approved; plus AI-unreviewed when AI is used). AI-assistance provenance (that AI was used and on what source) is required ONLY when AI is used. | Supports BR-006, FR-023, FR-031. |

## Explicitly out of scope here

- Field types, lengths, keys, indexes, relationships, normalisation.
- Storage format, identifiers implementation, API request/response shapes.
- Any real or synthetic application data instances (data population is a later phase).

## Open questions (information level)

- OQ-I1: RESOLVED — request and opportunity case are distinct concepts, one opportunity case per request for the MVP unless later validation shows a need for split/merge (see Core business concepts above).
- OQ-I2: What is the minimum information set for the pre-build validation prototype vs the full model above? (see MVP_BOUNDARY.md)
