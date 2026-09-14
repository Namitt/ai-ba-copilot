# Business Rules and Decision Controls

Status: APPROVED
Owner: Namit Singh
Phase: 3 — Product Requirements
Basis: BA_OPERATING_MODEL; OPPORTUNITY_LIFECYCLE; TO_BE_PROCESS; PRIORITISATION_APPROACH; RACI.

> APPROVED — owner-approved as part of the Phase 3 Product Requirements baseline on 2026-09-14, after initial draft, owner CONDITIONAL PASS, amendments and final consistency review. Approval accepts this artefact as the current requirements baseline; it does NOT authorise a software build, Phase 4, or the pre-build validation gate (Phase 3.5). Prior review note: A business rule states what must GOVERN the process; it is not implementation logic. None of these rules specifies a database trigger, workflow engine, code or technology — architecture (Phase 5) decides how each is enforced. These rules encode the approved control model and are, unless noted, non-negotiable (derive from locked principles or approved process), not hypotheses.

| ID | Business rule | Category | Source | Enforced by (class) |
|---|---|---|---|---|
| BRULE-001 | A request must have a named business/operational decision owner before it can progress beyond triage. | Owner / progression gate | LC-001; SR-004 | DET check + HUMAN naming |
| BRULE-002 | An unresolved specialist hard blocker (legal, policy, privacy, data-permission, technical-permission) must prevent progression of the affected action. | Hard gate | BACT-004; LC-004; SR-008 | DET gate; specialist clears |
| BRULE-003 | Assessed value must not override or offset an unresolved hard gate; a high score cannot pass a blocker. | Prioritisation control | PRIORITISATION | DET |
| BRULE-004 | AI-generated content remains "unreviewed" until a human reviews it and cannot confer approval; a completeness check is not substantive approval. | AI control | DEC-002; EV-007 | DET marking + HUMAN review |
| BRULE-005 | A field with no evidence must remain "unknown"; it must not be auto-populated or inferred as fact. | Evidence integrity | RSK-004; BR-002 | DET |
| BRULE-006 | A blocked, parked or stopped opportunity must not silently progress; PARK retains a revisit trigger and STOP retains a reason; neither deletes the record. | State integrity | SCN-003/004; LC-006 | DET |
| BRULE-007 | An early triage governance referral must return to the appropriate discovery/options route; it must not skip to option-specific (LC-004) assurance or bypass problem understanding and options. | Routing control | TO-BE routing fix | DET workflow |
| BRULE-008 | A material change to purpose, data, decision effect, cost or ownership must reopen the relevant decision gate; a prior approval is not blanket clearance for changed scope. | Change control | TO-BE traceability | DET rule + HUMAN |
| BRULE-009 | Every progression decision must record the accountable authority, rationale, conditions and any dissent. | Decision record | LC-006; RACI | DET + HUMAN |
| BRULE-010 | A superseded decision or record must be retained with its reason, not deleted. | Retention | TO-BE | DET |
| BRULE-011 | Exactly one accountable authority per bounded decision or disposition; a single opportunity may require several distinct authorised dispositions (e.g. technical, privacy/governance, financial, portfolio/business), which are not collapsed into one. The BA recommends but does not hold technical, finance, governance, delivery or operational authority. | Authority separation | RACI | DET + governance |
| BRULE-012 | Non-AI route, refine, more-evidence, park and stop must remain valid outcomes at the relevant gates; the process must not force an AI solution. | Outcome integrity | SCN-002/003/004; TO-BE | DET workflow |

## Business rule vs implementation (illustration)

- Rule (BRULE-002): "An unresolved specialist hard blocker must prevent progression of the affected action." — this is the rule.
- NOT a rule (deferred to Phase 5): how the block is stored, whether a state machine or a validation service enforces it, what the API contract is. Phase 3 does not decide these.

## Notes

- BRULE-002/003/004/005/006 are the load-bearing safety controls; they map directly to FR-012, FR-018, FR-026, FR-005, FR-021 and to acceptance criteria in USER_STORIES_AND_AC.md.
- All rules are stated for the demonstration context and are non-legal-advice; STK-06 determines applicable assurance constraints per opportunity.

## Open questions (rules level)

- OQ-R1: Should BRULE-001 (named owner before progression) block at triage or only at the first funding/assurance gate? (owner decision)
- OQ-R2: Are these rules better demonstrated as enforced software constraints or as a documented governance checklist for the pre-build validation prototype? (see MVP_BOUNDARY.md)
