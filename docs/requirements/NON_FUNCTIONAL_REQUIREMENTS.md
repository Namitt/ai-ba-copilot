# Non-Functional Requirements

Status: APPROVED
Owner: Namit Singh
Phase: 3 — Product Requirements
Basis: PRODUCT_VISION principles; F-D1 governance; DEC-003; RACI; RSK-004/006/010.

> APPROVED — owner-approved as part of the Phase 3 Product Requirements baseline on 2026-09-14, after initial draft, owner CONDITIONAL PASS, amendments and final consistency review. Approval accepts this artefact as the current requirements baseline; it does NOT authorise a software build, Phase 4, or the pre-build validation gate (Phase 3.5). Prior review note: Only NFRs justified from the approved baseline are stated. **No numeric target is invented.** Where a measurable target would be needed but no evidence supports a number, it is recorded as **TARGET TO BE VALIDATED** with why it matters, who should validate it, and when it must be resolved. Security/performance standards are not asserted beyond what the baseline supports.

| ID | Non-functional requirement | Rationale / source | Measurable target | Priority |
|---|---|---|---|---|
| NFR-001 | Traceability & auditability: every material record links to its source and prior versions and is retained (not deleted). | BR-006; PP-007; governance expectation | Qualitative (chain navigable; superseded retained). No numeric target needed. | MUST |
| NFR-002 | AI transparency: whenever AI-generated content exists, it is always distinguishable and attributable, and marked unreviewed until human review. | BR-008; EV-007; RSK-004 | Qualitative (all AI outputs marked — a control, not a tuned metric). | CONDITIONAL MUST — IF AI ENABLED |
| NFR-003 | Authority-based access control: an action is permitted only to a role with the legitimate authority for it. | RACI; BRULE-011 | Roles/authorities enumerated; unauthorized action prevented. Specific access model TARGET TO BE VALIDATED (who validates: STK-06 + owner; when: before build). | MUST |
| NFR-004 | Privacy / data protection by design: governance fields captured early; personal data minimised; DPIA-trigger and ADM-safeguard capture; non-legal-advice. | ASM-007; F-D1; EV-004/005/013 | Governance field set present; specific retention/DP controls TARGET TO BE VALIDATED (who: STK-06; when: before handling any non-synthetic data). | MUST |
| NFR-005 | Provider independence: workflow state must not depend on any single AI provider. | DEC-003; ASM-008; RSK-006 | Qualitative (state persists independent of provider). | SHOULD |
| NFR-006 | Deterministic computation: calculations, validation rules and workflow state are deterministic and reproducible. | PRODUCT_VISION; PRIORITISATION arithmetic | Same inputs → same outputs; arithmetic reproducible. | MUST |
| NFR-007 | Proportionality / usability: recording burden is proportionate to opportunity risk and value; the discipline must not impose overhead that outweighs benefit. | ASM-002/004; RSK-009 | TARGET TO BE VALIDATED via real-user testing (who: STK-02/08 + owner; when: Phase 4/validation). Directly tests ASM-004. | MUST |
| NFR-008 | Reliability & recoverability of records: records are not lost and can be recovered. | BR-006; RSK-008 | TARGET TO BE VALIDATED (who: owner/Phase 5; when: before build). No invented uptime figure. | SHOULD |
| NFR-009 | Security of stored records: records are protected against unauthorised access/tampering. | Governance; RACI | Standards TARGET TO BE VALIDATED (who: STK-06/owner; when: before any real data). No invented standard asserted. | SHOULD |
| NFR-010 | Accessibility: if software is built, it should be usable by people with a range of abilities. | CANDIDATE — **NO TRACEABLE JUSTIFICATION** in the approved Phase 1/2 baseline; retained honestly pending an authorised phase establishing the applicable requirement. Not "polish". | Applicable standard/target TARGET TO BE VALIDATED (who: authorised UX/validation phase; when: before build). No standard, version or legal basis selected here. | CANDIDATE / SHOULD (pending validation) |
| NFR-011 | Maintainability & portability: the discipline and its records should be portable and not locked to one vendor/tool where avoidable. | DEC-003/004; free-first | Validation method: a portability/maintainability acceptance approach (how portability will be demonstrated) must be defined before architecture/build commitment; no architecture chosen here. | SHOULD |

## Fabrication guard (explicit)

No uptime %, response-time, retention-day, concurrency or throughput number is stated, because the approved baseline supports none. Every place such a number would normally appear is recorded as TARGET TO BE VALIDATED. Inventing these would breach the project's evidence discipline (RSK-008). NFR-010 (accessibility) is retained honestly as a CANDIDATE with NO TRACEABLE JUSTIFICATION in the approved baseline — not dropped and not falsely sourced.

## Open questions (NFR level)

- OQ-N1: Which NFR targets must be resolved before the pre-build validation prototype (synthetic data only) vs before any handling of real data?
- OQ-N2: Is NFR-007 (proportionality) the single most important NFR to test, since it directly probes ASM-004 (adoption) and RSK-009 (over-engineering)?
