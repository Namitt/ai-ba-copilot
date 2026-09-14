# Track A No-Code Validation Prototype Spec

Status: APPROVED
Owner: Namit Singh
Phase: 3.5 — Pre-Build Validation
Basis: approved Phase 3 requirements; OPPORTUNITY_LIFECYCLE (LC); BA_OPERATING_MODEL (BACT).

> **APPROVED — Phase 3.5 validation-design baseline (2026-09-14; DEC-013).** Approval followed owner CONDITIONAL PASS, amendment cycles and a final consistency/terminology cleanup; it authorises this design as the current baseline and does **NOT** authorise participant execution, the dry run, Track B, Phase 4 or a build. This specifies **no-code artefacts** (structured documents/templates + a lightweight log) for Track A. It is NOT application/UX design — no screens, layouts, widgets, navigation, styling, architecture, stack or code. The prototype is deliberately **lighter than the full Phase 3 requirement catalogue**; NFR-007 (proportionality) is itself under test, so every element must earn its place.

## 0. The two conditions this spec supports (fair comparison)

Track A compares two ways of working on **matched-but-different** scenarios of comparable difficulty (VALIDATION_PLAN §2 — not the same underlying scenario twice; a scenario's fixed information set does not vary by which condition it is assigned to):
- **Condition A — credible current practice (baseline, NOT a strawman):** the participant's **natural analysis approach** or a plain unstructured worksheet / ordinary notes, applied to the assigned case, with **none** of the Phase 3.5 structured prompts, explicit gates, traceability structure or governance checklist. It is not a blank page and is not deliberately impoverished.
- **Condition B — structured discipline:** the lightweight structured artefacts specified below, applied to the matched case.

**No privileged information on either side.** Neither condition receives extra evidence unavailable to the other, and Condition B adds **no configured workflow software**; the only intended difference is the structured discipline itself. Any configured-tool capability belongs to **Track B**, not here.

## 1. Form

Plain documents/tables a participant can fill in (e.g. a single structured template per opportunity case plus one running log), usable on paper or in any generic editor/spreadsheet. **No configured workflow software (e.g. a set-up Jira/Notion workflow) is used in Track A — that is Track B.** No tool is prescribed.

## 2. Minimum elements (challenged for necessity)

| # | Element | Purpose (approved link) | Keep? / challenge |
|---|---|---|---|
| 1 | Opportunity-case header | request; stated problem vs requested solution; intended decision/use; owner (LC-001; BR-001) | KEEP — core of the discipline |
| 2 | Evidence & unknown log | claims with references; explicit "unknown"; gaps (LC-002; BR-002; BRULE-005) | KEEP — tests evidence discipline |
| 3 | Options comparison | AI-applicability considered; AI (if credible) vs non-AI vs no-change; retained rejects (LC-003; BR-003) | KEEP — tests anti-solutioning & non-AI |
| 4 | Governance checkpoint | personal-data/DPIA trigger, ADM level, oversight, fairness, accountable owner; disposition passed/conditions/blocked (LC-004; BR-004) | KEEP — tests governance-forward + blockers |
| 5 | Gate vs ranking record | hard gates separate from ranking inputs; value cannot offset a blocker (LC-005; BR-007) | KEEP — tests the no-override control |
| 6 | Recommendation & decision record | recommendation (not approval); decision route — one of PROCEED / NON-AI ROUTE / REFINE / MORE EVIDENCE REQUIRED / PARK / STOP / ESCALATE GOVERNANCE; rationale; accountable authority; conditions (LC-005/006; BR-008/009). A blocked/held activity is a consequence/state pending specialist disposition, **not** a separate route (no HOLD route). | KEEP — tests decision clarity & routes |
| 7 | Traceability view | one-line chain request→evidence→options→governance→decision (BR-006) | KEEP but MINIMAL — a single reference column, not a system |

Deliberately EXCLUDED from Track A: AI assistance (FR-003/009/026-029), detailed value baseline / expected-vs-actual measurement (BR-005/FR-014-016), portfolio/dashboards, automated evidence, any screen or workflow engine. These would confound ASM-002/ASM-004 or exceed the prototype's purpose.

## 3. Proportionality guardrails

- One page per case where feasible; the log is shared across cases.
- No field is mandatory merely to "complete the template"; a field left "unknown" is a valid, expected outcome.
- Burden and time are measured (they are evidence about NFR-007/ASM-004), not minimised by hiding steps.
- If a participant can achieve the same decision quality with fewer elements, that is a finding, not a failure.

## 4. Not in scope

No UI mockups, wireframes, components, navigation, styling; no data model/schema; no tool selection; no code. Any eventual software design is Phase 4+, and only if authorised.
