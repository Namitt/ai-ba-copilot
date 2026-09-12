# AS-IS Hypothesis Stress Test

Status: APPROVED
Owner: Namit Singh
Phase: 2
Baseline: approved AS_IS_PROCESS.md at fb5f23f / closure 3cdbcce; unchanged.

> Owner-approved as part of the Phase 2 BA operating-model baseline on 2026-09-11 (content commit 2f7f09d). Approval accepts this stress test as the current project baseline; it does not make the synthetic stress test real-world validation, and the OPEN assumptions remain.

## Method

Manual desk walk-through of SCN-001..004 in SYNTHETIC_SCENARIOS.md. Each cell tests the failure mode against stipulated inputs, including counterexamples. No interviews, pilot, user test or empirical industry validation occurred. SCENARIO-SUPPORTED means a case exhibits the proposed mechanism by construction; it does not establish prevalence, causation or efficacy. CHALLENGED means a supplied counterexample limits the claim, not that the failure can never occur. PLAUSIBLE BUT NOT TESTED means relevant but no premise permits a conclusion. NOT RELEVANT means outside this case's exercised scope, not universally irrelevant.

## Every Phase 1 failure mode

| ID | SCN-001 support | SCN-002 purchasing | SCN-003 hardship | SCN-004 dashboard | Overall interpretation and process response |
|---|---|---|---|---|---|
| PP-001 inconsistent intake/framing | SCENARIO-SUPPORTED: E2 category ambiguity mixes policy and language problems | SCENARIO-SUPPORTED: E1 missing fields | CHALLENGED: established assessment policy exists; backlog does not establish poor intake | SCENARIO-SUPPORTED: no decision or action owner | Mixed. Separate request from problem; accept adequate existing records rather than recreate intake. |
| PP-002 solutioning before evidence/options | SCENARIO-SUPPORTED: AI requested before labels/causes checked | SCENARIO-SUPPORTED: AI requested despite explicit rules and absence delays | SCENARIO-SUPPORTED: rejection automation requested with no fairness/label assessment | SCENARIO-SUPPORTED: dashboard proposed before its use | Mechanism supported within cases; no frequency claim. Require meaningful non-AI and do-nothing comparison. |
| PP-003 missing baseline/value definition | SCENARIO-SUPPORTED: transfer/time data do not establish avoidable loss | SCENARIO-SUPPORTED: delays counted but chasing/cost not measured | SCENARIO-SUPPORTED: stock of 300 pending is not throughput/benefit evidence | SCENARIO-SUPPORTED: no beneficiary/value proposition | Partial data is not a value baseline. Record denominator, observation period, gaps and measurement owner. |
| PP-004 inconsistent prioritisation | PLAUSIBLE BUT NOT TESTED: no comparative portfolio decisions supplied | PLAUSIBLE BUT NOT TESTED: competing demand unspecified | PLAUSIBLE BUT NOT TESTED: urgency alone does not demonstrate inconsistency | PLAUSIBLE BUT NOT TESTED: sponsor preference supplied, no historical ranking | Not tested. Cross-case prioritisation below is a proposed intervention, not evidence of historic inconsistency. |
| PP-005 late governance | PLAUSIBLE BUT NOT TESTED: review missing, timing of actual engagement unspecified | CHALLENGED: approved controls/routing exist before change | CHALLENGED: E3 explicitly places privacy escalation at intake | NOT RELEVANT: no processing change exercised | Blanket late-governance narrative challenged. Screen early, reuse existing assurance, reopen on material data/purpose change. |
| PP-006 adoption/outcome not measured | PLAUSIBLE BUT NOT TESTED: no deployed change observed | PLAUSIBLE BUT NOT TESTED: no changed process observed | PLAUSIBLE BUT NOT TESTED: no proposed automation deployed | SCENARIO-SUPPORTED: existing summary lacks recorded readership/action | One illustrative case only. Define later measurement handoff now; do not pretend future adoption was tested. |
| PP-007 no end-to-end traceability | CHALLENGED: ticket IDs/category guide provide partial traceability | CHALLENGED: approval decision record exists | CHALLENGED: human reasons/escalation recorded | SCENARIO-SUPPORTED: no link from output to action | Universal absence challenged; full end-to-end completeness remains untested in first three. Extend references, do not duplicate records. |

## Challenge to the assumed sequence

The Phase 1 intake-to-pilot sequence cannot be universal: SCN-003 already has governance at entry; SCN-002 has operational control and may need a simple non-AI change; SCN-004 may stop before option appraisal. Stakeholder mapping and assurance must recur. Adoption/integration may still prevent value after perfect intake (SCN-001), so front-end process repair is not sufficient proof for ASM-010.

## Verification and limits

All seven PP identifiers classified in all four cases (28 explicit classifications). Findings are internally stress-tested only. The approved AS-IS was preserved; these results are a companion stress test to it. Next empirical validation: practitioner comparison of current request handling, actual records and exceptions, with consent and approved data access. No such access is assumed.
