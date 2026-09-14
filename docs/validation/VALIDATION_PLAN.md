# Phase 3.5 Validation Plan (Track A design)

Status: APPROVED
Owner: Namit Singh
Phase: 3.5 — Pre-Build Validation
Basis: PHASE3_5_CHARTER.md; approved Phase 1–3 baselines.

> **APPROVED — Phase 3.5 validation-design baseline (2026-09-14; DEC-013).** Approval followed owner CONDITIONAL PASS, amendment cycles and a final consistency/terminology cleanup; it authorises this design as the current baseline and does **NOT** authorise participant execution, the dry run, Track B, Phase 4 or a build. Design of Track A only. Track A is **NOT STARTED**; no participants recruited; no results claimed. Directional product/process validation — not a clinical experiment and not statistical proof.

## 1. Objective (Track A)

Obtain directional evidence on whether the **structured BA operating discipline** changes observable decision quality (ASM-002) and whether practitioners will use it without disproportionate burden (ASM-004) — **without** AI and **without custom or configured workflow software**, so the variable under test is the discipline itself, not more information or better tooling.

## 2. The variable under test (fair comparison)

The only intended difference between conditions is **structured discipline** — not information availability and not tooling. The experimental rule that enforces this:

- **Each scenario brief has a fixed information set.** A scenario's facts and source material do **not** change depending on whether that scenario is assigned to Condition A or Condition B.
- **Within a participant, A and B use matched-but-different scenarios** — not the same underlying scenario twice. Matched cases have **comparable** information quantity, quality, ambiguity and difficulty, but their facts are **not literally identical**.
- **Neither condition receives additional evidence unavailable to the other** merely because of the condition (no privileged information; no configured tool on one side only).
- **Condition B differs through STRUCTURE**, not privileged information or tooling.

Conditions:
- **Condition A (credible current practice — NOT a blank page):** the participant analyses the assigned case using their **natural analysis approach** / ordinary notes / a lightweight unstructured worksheet. It must **not** contain the Phase 3.5 structured prompts, explicit gates, traceability structure or governance checklist. It represents what a competent practitioner would do today.
- **Condition B (structured discipline):** the participant analyses the matched case using the lightweight structured Phase 3.5 no-code prototype (VALIDATION_PROTOTYPE_SPEC.md) — structured for analysis, with **no extra evidence** and **no configured workflow software**.

If either condition received extra facts or a configured tool the other lacked, the study would test information/tooling, not discipline — that is explicitly disallowed (see §10).

## 3. Design — within-participant comparative validation

Each participant works **matched but different** synthetic cases under both conditions.

- **Per participant: ~2 matched pairs = ~4 cases total** (subject to the dry run confirming this is manageable). In each pair, one case is done under Condition A and its matched equivalent under Condition B.
- **Counterbalancing (AB/BA):** vary which condition comes first across participants; vary which case of a pair is A vs B.
- **No repeat of the same underlying scenario** to the same participant — always matched-but-different cases.
- **Scenario rotation:** different participants may receive different pairs from the broader SCN bank (SCENARIO_PLAN.md) to obtain coverage.

### 2.1 Order, learning, fatigue, carryover (explicitly addressed)
- Order effects: AB/BA counterbalancing.
- Learning effects: because a participant may get better at the *task* after Condition B, any later-Condition-A improvement is a recognised risk — it is **recorded** and factored into interpretation, not ignored. Counterbalancing distributes this across participants.
- Fatigue: ~4 cases per participant caps session length; the dry run estimates realistic duration; breaks allowed.
- Carryover: matched-but-different cases reduce direct carryover; residual carryover is noted as a limitation.

## 4. What Track A observes

Scored via the grouped rubric (SCORING_RUBRIC.md), dimensions A–F: problem/evidence discipline; option quality; governance/control; decision/authority quality; traceability/rationale; burden/adoption. Structural (objective) observations are kept separate from subjective feedback. No success percentages are invented.

## 5. Scenario matching (reviewed before testing)

Cases in a pair must be reasonably matched on: complexity, information volume, ambiguity, governance difficulty and decision difficulty. **Perfect equivalence is not claimed.** Before any session, the owner (and, where practical, a second reviewer) reviews each pair for equivalence and for bias; mismatches are rebalanced or the pair is dropped. Matching review is recorded.

## 6. Pre-test dry run (mandatory)

A **dry-run/pilot session runs before any evidence collection** to verify instructions, detect confusing wording, check scenario difficulty, estimate session length, surface rubric ambiguity, gauge prototype burden, and check whether participants can infer the desired answer. **Default: the dry run is EXCLUDED from the Track A evidence set.** It may be included only if the protocol was unchanged AND the owner explicitly approves inclusion. Any material protocol change after the dry run is recorded before formal sessions start.

## 7. Session outline (per participant)

1. Neutral briefing + lightweight consent (PARTICIPANT_PLAN.md) — no leading language; "we are testing the process, not you".
2. Work the assigned matched cases under the counterbalanced conditions; capture outputs, time, notes. Facilitator does not coach or reveal expected answers.
3. Short structured feedback (burden, usefulness, willingness) — kept separate from structural scoring.
4. Preserve the **raw participant outputs before any debrief interpretation**; anonymise by participant ID.

## 8. Bias controls (summary; see SCORING_RUBRIC + PARTICIPANT_PLAN)

Rubric, scenario expectations and protocol are fixed before sessions; facilitator stays neutral; raw output preserved pre-debrief; outputs anonymised and, where practical, scored without reliance on which condition the project hopes will win; optionally a second reviewer scores a subset and disagreements are recorded (no formal inter-rater reliability claimed unless actually measured).

## 9. Analysis (Track A)

Compare Condition A vs B per rubric dimension across participants; summarise directionally (counts/patterns, not p-values), separating structural results from subjective feedback; record limitations (small n, synthetic, learning/carryover). Feed into the pre-committed qualitative GO/MODIFY/STOP matrix (PHASE3_5_CHARTER §5). Output artefacts (results/analysis) are created only when Track A runs — currently **NOT STARTED**.

## 10. Boundaries

A scenario's fixed information set does not vary by assigned condition, and neither condition receives privileged evidence (matched-but-different cases per §2); Condition B adds no extra evidence and no configured workflow software; no AI; no custom software; no UX; no architecture/stack/provider; synthetic only; existing SCN family. Track B (existing-tool sufficiency) is planned separately and runs only after Track A **and** a further owner gate (TRACK_B_TOOL_EVALUATION_PLAN.md).
