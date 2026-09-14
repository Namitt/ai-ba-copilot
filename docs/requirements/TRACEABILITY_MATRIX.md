# Requirements Traceability Matrix

Status: APPROVED
Owner: Namit Singh
Phase: 3 — Product Requirements

> APPROVED — owner-approved as part of the Phase 3 Product Requirements baseline on 2026-09-14, after initial draft, owner CONDITIONAL PASS, amendments and final consistency review. Approval accepts this artefact as the current requirements baseline; it does NOT authorise a software build, Phase 4, or the pre-build validation gate (Phase 3.5). Prior review note: Links approved needs (Evidence/PP/ASM/RSK/STK, and lifecycle LC / activity BACT) to BR → SR → FR/NFR/BRULE → US → AC. Links reflect real dependency; none are added to fill cells. Any requirement without a justified source is marked **NO TRACEABLE JUSTIFICATION** and must not silently remain MUST. Result: one requirement (NFR-010, accessibility) is deliberately retained as NO TRACEABLE JUSTIFICATION / CANDIDATE pending an authorised phase; it is not classified MUST (see §4a and §7).

## 1. Need → Business Requirement

| Approved need | BR |
|---|---|
| PP-001 inconsistent intake; PP-002 solutioning first; F-A3 | BR-001 |
| PP-003 missing baseline/value; RSK-003/004 evidence/AI risk | BR-002 |
| PP-002; F-E2; SCN-002 | BR-003 |
| PP-005 late governance; F-D1; ASM-007; STK-06 | BR-004 |
| PP-003/006; F-C1/C2; ASM-006; EV-012 | BR-005 |
| PP-007 no traceability; F-B2; RSK-008 | BR-006 |
| PP-004 inconsistent prioritisation; F-A2; PRIORITISATION | BR-007 |
| F-B1; EV-007; DEC-002 | BR-008 |
| SCN-002/003/004; TO-BE | BR-009 |

## 2. BR → SR

| BR | SR |
|---|---|
| BR-001 | SR-001 |
| BR-002 | SR-002 |
| BR-003 | SR-003, SR-006 |
| BR-004 | SR-008 |
| BR-005 | SR-007, SR-010 |
| BR-006 | SR-004, SR-009 |
| BR-007 | SR-005 |
| BR-008 | (all SR; control model) |
| BR-009 | SR-004 |

## 3. BR/SR → FR / NFR / BRULE

| BR/SR | FR | NFR | BRULE |
|---|---|---|---|
| BR-001 / SR-001 | FR-001, FR-002, FR-003 | — | BRULE-001 |
| BR-002 / SR-002 | FR-004, FR-005, FR-006 | NFR-002 | BRULE-005 |
| BR-003 / SR-003,006 | FR-007, FR-008, FR-009 | — | BRULE-010, BRULE-012 |
| BR-004 / SR-008 | FR-010, FR-011, FR-012, FR-013 | NFR-004 | BRULE-002, BRULE-007 |
| BR-005 / SR-007,010 | FR-014, FR-015, FR-016 | NFR-006 | — |
| BR-006 / SR-004,009 | FR-022, FR-023, FR-024, FR-025, FR-031 | NFR-001, NFR-008 | BRULE-008, BRULE-009, BRULE-010 |
| BR-007 / SR-005 | FR-017, FR-018, FR-019 | — | BRULE-003 |
| BR-008 / all | FR-026, FR-027, FR-028, FR-029, FR-030 | NFR-002, NFR-005 | BRULE-004 |
| BR-009 / SR-004 | FR-020, FR-021 | — | BRULE-006, BRULE-012 |
| (authority) RACI | FR-032 | NFR-003 | BRULE-011 |

## 4. FR → US → AC (principal)

| FR group | US | AC |
|---|---|---|
| FR-001/002/003 | US-001, US-004 | AC-001/002, AC-009..012 |
| FR-004/005/006 | US-002 | AC-003/004/005 |
| FR-007/008/009 | US-003 | AC-006/007/008 |
| FR-010/011 | US-005 | AC-013/014 |
| FR-012/018 | US-006 | AC-015/016 |
| FR-013 | US-007 | AC-017/018 |
| FR-017/019 | US-008 | AC-019/020 |
| FR-020/021/022/025 | US-009 | AC-021/022/023 |
| FR-014/015/016 | US-010 | AC-024/025 |
| FR-023/024/031 | US-011 | AC-026/027 |
| FR-032 | US-012 | AC-028 |

## 4a. NFR traceability (explicit)

| NFR | Traces to | Note |
|---|---|---|
| NFR-001 traceability/audit | BR-006; PP-007 | — |
| NFR-002 AI transparency | BR-008; EV-007 | CONDITIONAL — applies when AI enabled |
| NFR-003 authority access | RACI; BRULE-011 | via FR-032 |
| NFR-004 privacy by design | F-D1; ASM-007; EV-004/005/013 | — |
| NFR-005 provider independence | DEC-003; RSK-006 | — |
| NFR-006 deterministic computation | PRODUCT_VISION; PRIORITISATION | — |
| NFR-007 proportionality/usability | ASM-002/004; RSK-009 | target to be validated |
| NFR-008 reliability/recoverability | BR-006; RSK-008 | target to be validated |
| NFR-009 security of records | governance expectation; RACI | target to be validated |
| NFR-010 accessibility | **NO TRACEABLE JUSTIFICATION** in approved Phase 1/2 baseline | CANDIDATE — retained honestly; applicable requirement to be set by an authorised phase |
| NFR-011 maintainability/portability | DEC-003/004; free-first | validation method to be defined before build |

## 5. Lifecycle / activity coverage (where genuinely applicable)

| LC / BACT | Requirements |
|---|---|
| LC-001 / BACT-001 triage | FR-001, FR-013; BRULE-001 |
| LC-002 / BACT-002 evidence | FR-004/005/006; BRULE-005 |
| LC-003 / BACT-003 options | FR-007/008/009; BRULE-010/012 |
| LC-004 / BACT-004 assurance | FR-010/011/012; BRULE-002/007 |
| LC-004/005 / BACT-005 value | FR-014/015/016 |
| LC-005 / BACT-006 prioritise | FR-017/018/019; BRULE-003 |
| LC-006 / BACT-007 decide | FR-020/021/022/025; BRULE-006/008/009 |

## 6. Assumption / risk coverage

| ASM / RSK | Addressed / tested by |
|---|---|
| ASM-002 (BA discipline improves outcomes — OPEN) | The whole requirement set is the hypothesis-under-test; NFR-007 proportionality probes it. Not proven by these requirements. |
| ASM-010 (intake drives value gap — OPEN) | BR-001/007 target intake/qualification; remains OPEN — requirements do not validate it. |
| ASM-006 (baselines obtainable — OPEN) | BR-005 / FR-014 flagged NEEDS VALIDATION. |
| ASM-004 (adoption — OPEN) | NFR-007; product-necessity challenge; requires real-user testing. |
| RSK-004 (AI inaccuracy) | BRULE-004/005; FR-005/026/029. |
| RSK-008 (overclaim) | NFR "fabrication guard"; NEEDS VALIDATION flags. |
| RSK-009 (over-engineering) | MVP_BOUNDARY product-necessity challenge; NFR-007. |

## 7. Justification check (honest)

Every FR and BRULE, and all NFRs except NFR-010, trace to at least one BR/SR and an approved Phase 1/2 need. **One requirement is deliberately retained without an approved source and is marked NO TRACEABLE JUSTIFICATION: NFR-010 (accessibility)** — kept honestly as a CANDIDATE pending an authorised phase that establishes the applicable requirement; it is not classified MUST and is not falsely sourced.

Requirements whose *necessity for a build* is unproven are flagged NEEDS VALIDATION (FR-003, FR-009, FR-014; the AI-assist niceties FR-026..029 as CONDITIONAL MUST — IF AI ENABLED) and are NOT classified unconditional MUST on that basis. Measurement (BR-005; FR-014..016) is SHOULD, not required for the pre-build validation prototype.
