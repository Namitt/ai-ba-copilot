# Track A Scoring / Review Rubric

Status: APPROVED
Owner: Namit Singh
Phase: 3.5 — Pre-Build Validation

> **APPROVED — Phase 3.5 validation-design baseline (2026-09-14; DEC-013).** Approval followed owner CONDITIONAL PASS, amendment cycles and a final consistency/terminology cleanup; it authorises this design as the current baseline and does **NOT** authorise participant execution, the dry run, Track B, Phase 4 or a build. This rubric is fixed **before** any participant testing. It assesses **observable decision quality and defensible reasoning**, not whether a participant reaches one pre-selected "correct" answer. Indicators are grouped into a manageable set of dimensions (A–F). Each indicator is coded **0/1** (or **0/1/2** where noted), never rolled into a single composite "magic score", and a **missed hard blocker is always flagged independently** of any aggregate.

## 1. Per-scenario preparation (done before testing, per SCN)

For each scenario the facilitator pre-records (from the scenario brief), so scoring is not invented live:
- evidence gaps expected to be noticed
- key assumptions in play
- credible alternative routes (incl. non-AI / no-change)
- governance/assurance concerns present
- **hard blocker(s), if any** (drives the independent blocker flag in §4)
- authority boundaries (which bounded dispositions apply)
- traceability expectations
- decision-quality characteristics of a defensible outcome (which may be several)

## 2. Grouped scoring dimensions (structural / objective)

Indicators are recorded **per case, per condition**, with a short evidence note (what the participant actually did). Coding is per-indicator; **dimensions are reported as indicator profiles, not summed into one overall number.** Where an indicator is coded 0/1/2, 0 = not done, 1 = partial, 2 = clearly done; otherwise 0/1 (not observed / observed).

### A. Problem / evidence discipline
- A1. Separated the stated problem from the requested solution (0/1/2)
- A2. Surfaced missing evidence and marked unknowns; did **not** invent facts (0/1/2)
- A3. Distinguished evidenced claims from assumptions (0/1)

### B. Option quality
- B1. Considered AI applicability explicitly (0/1)
- B2. Considered a credible non-AI / no-change alternative (0/1/2)
- B3. Resisted "AI because AI" where AI was not warranted (0/1)

### C. Governance / control
- C1. Identified the governance/assurance concerns present (0/1/2)
- C2. Identified the hard blocker(s) present (0/1) — **also drives the independent flag in §4**
- C3. Kept hard gates separate from value/ranking; did not let value override a blocker (0/1)

### D. Decision / authority quality
- D1. Reached a clear recommendation, marked as recommendation (not approval) (0/1)
- D2. Used an appropriate route (PROCEED / NON-AI ROUTE / REFINE / MORE EVIDENCE REQUIRED / PARK / STOP / ESCALATE GOVERNANCE) with reason (0/1). *(Where a blocker exists, the defensible route is typically ESCALATE GOVERNANCE or STOP; separately, the affected action being blocked/held pending specialist disposition is a consequence/state of the blocker, not a distinct decision route.)*
- D3. Named the accountable authority / bounded disposition(s) (0/1)

### E. Traceability / rationale
- E1. Gave a defensible rationale for the recommendation/route (0/1/2)
- E2. Traced key claims to their evidence (0/1)

### F. Burden / adoption (mixed objective + participant-reported; kept separate from A–E)
- F1. Time/effort per case (measured, minutes)
- F2. Perceived burden (participant; simple ordinal or short comment)
- F3. Perceived usefulness (participant)
- F4. Willingness to use again (participant)

F is not scored as decision quality; it is the ASM-004 / NFR-007 (proportionality) evidence and is read alongside A–E, not blended into them.

## 3. Reporting model (no composite magic score)

- Report each condition as an **indicator profile** across A–E (which indicators were observed), plus the F burden/adoption measures — per participant and in aggregate (counts/patterns).
- Do **not** produce a single total that could let strong performance on one dimension hide a failure on another.
- If an aggregate view is wanted, it is a **per-dimension** summary (e.g. "how many cases surfaced unknowns"), never one number across dimensions.

## 4. Independent hard-blocker flag (never averaged away)

For any scenario that contains a hard blocker, indicator **C2** (blocker identified) and **C3** (value did not override it) are reported **on their own**, visibly, regardless of every other indicator. A participant who scores well on A, B, D, E but **misses the blocker (C2 = 0)** is reported as *missed the blocker* — this is never offset or hidden by other dimensions.

## 5. Defensible-reasoning principle

Where multiple reasonable decisions exist, score the **reasoning** (A–E), not the label of the outcome. A participant who PARKs with sound reasoning scores as well as one who proceeds with sound reasoning, if both are defensible for that scenario. The rubric rewards defensible judgement, not filling every field or reaching one prescribed answer.

## 6. Bias controls tied to scoring

- The rubric, per-scenario expectations and protocol are **fixed before** any session.
- Raw participant output is preserved **before** any debrief interpretation; scoring works from the raw output.
- Outputs are anonymised (participant ID) and, where practical, scored without leaning on which condition the project hopes will win (blind-ish).
- **Optionally** a second reviewer scores a subset; disagreements are recorded. **No inter-rater reliability statistic is claimed unless it is actually measured.**

## 7. Thresholds (OWNER-APPROVED BEFORE TESTING — default is qualitative)

No numeric thresholds are fabricated here, and **numeric GO/MODIFY/STOP thresholds are NOT used** unless the owner explicitly writes and approves them into this section, with justification, **before** any session. Default: the GO/MODIFY/STOP decision is a **documented qualitative judgement** against the A–F indicator profiles and the independent blocker flag, per the pre-committed decision matrix in PHASE3_5_CHARTER.md §5. A missed hard blocker (C2 = 0 on a blocker scenario) is always surfaced explicitly and is a material input to that judgement — it is never averaged away.
