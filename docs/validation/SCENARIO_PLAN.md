# Track A Scenario Plan (synthetic)

Status: APPROVED
Owner: Namit Singh
Phase: 3.5 — Pre-Build Validation
Basis: SYNTHETIC_SCENARIOS.md (SCN-001..004); AS_IS_VALIDATION stress test.

> **APPROVED — Phase 3.5 validation-design baseline (2026-09-14; DEC-013).** Approval followed owner CONDITIONAL PASS, amendment cycles and a final consistency/terminology cleanup; it authorises this design as the current baseline and does **NOT** authorise participant execution, the dry run, Track B, Phase 4 or a build. Matched **synthetic** scenarios for Track A. No Primark, no real/confidential organisation or data. Uses the existing **SCN** identifier family only; no new family. Scenarios are designed to be disconfirming (the disciplined answer is sometimes non-AI, PARK or STOP), so the design does not bias toward "the process wins". Full scenario briefs are drafted at execution time from these specs; none are run yet.

## 1. Design intent

Provide a **broader bank of matched scenario pairs** so that each participant works **~2 matched pairs = ~4 cases** (VALIDATION_PLAN §3), and different participants can be **rotated** across different pairs for coverage. Within each pair, the two cases are of **comparable difficulty** (complexity, information volume, ambiguity, governance difficulty, decision difficulty) so that one can be done under Condition A and its matched equivalent under Condition B without either condition being handed an easier case. The **same underlying scenario is never given twice** to the same participant. Collectively the bank must stress every behaviour the rubric scores. Phase 2's SCN-001..004 are reused as *lessons* but not copied verbatim where that would make validation artificial; new scenarios continue the SCN numbering (SCN-005 onward).

**Which condition gets which case of a pair is counterbalanced** across participants (AB/BA), so the discipline is not always tested on the same half of a pair (VALIDATION_PLAN §2.1).

## 2. Stressors to cover (across the set)

- credible AI opportunity
- credible non-AI alternative (AI not the best answer)
- weak evidence / unknown baseline
- material governance/assurance concern
- hard blocker (legal/policy/privacy/permission)
- high headline value that must NOT override a blocker
- tempting but weak "AI because AI" request
- legitimate PARK / STOP / MORE EVIDENCE REQUIRED outcome

## 3. Candidate scenario specs (synthetic; briefs written at execution)

| ID | Theme (synthetic) | Primary stressors | Disciplined "defensible" direction (not the only allowed answer) |
|---|---|---|---|
| SCN-005 | Support-triage assist request | credible AI; weak baseline/unknowns | MORE EVIDENCE before build; measure avoidable work first |
| SCN-006 | "Automate approvals" request | credible non-AI; existing rules/absence delays | NON-AI ROUTE / process fix; AI not warranted |
| SCN-007 | Consequential eligibility decisioning | governance concern; hard blocker; high headline value | ESCALATE GOVERNANCE (affected action blocked pending specialist disposition); value cannot override the blocker |
| SCN-008 | "Add a chatbot because competitors have one" | weak "AI because AI"; no decision owner/use | PARK or STOP; record the conclusion, no fictional value |
| SCN-009 | Reporting/insight request with real recurring decision | credible AI vs non-AI; adoption doubt | Compare options; MORE EVIDENCE on adoption; conditional |
| SCN-010 | Personal-data enrichment idea | privacy hard blocker; DPIA trigger | ESCALATE GOVERNANCE (affected action blocked pending specialist disposition); safe alternatives within scope |

(These 6 candidates seed the bank; the owner may trim or extend. They are paired at execution — e.g. two credible-AI-vs-non-AI cases form one matched pair, two blocker/governance cases another — so a participant gets ~2 pairs. **Each pair's equivalence is reviewed and recorded before testing** — see §4.) Each brief will include: request text, available (partial) evidence with deliberate unknowns, any embedded blocker, stakeholders/authorities, and a tempting-but-wrong path. A scenario's **fixed information set does not change by which condition it is assigned to**, and within a participant the two conditions use **matched-but-different** scenarios (not the same scenario twice); neither condition is given privileged evidence (VALIDATION_PLAN §2).

## 4. Anti-bias rules

- At least half the scenarios have a defensible NON-AI ROUTE / PARK / STOP / ESCALATE GOVERNANCE outcome, so "do the AI thing" is not rewarded.
- No scenario has a single prescribed "correct answer"; the rubric rewards defensible reasoning (SCORING_RUBRIC.md).
- **Matched-pair equivalence review (recorded):** before any session, the owner (and, where practical, a second reviewer) reviews each pair for equivalent difficulty, stressor coverage and bias. Perfect equivalence is **not** claimed; mismatched pairs are rebalanced or dropped, and the review is documented.
- Owner reviews the briefs for bias and realism before any session.

## 5. Boundaries

Synthetic only; SCN family only; no real data; no enterprise-prevalence claims. Scenarios test decision behaviour on constructed cases, not real-world outcomes.
