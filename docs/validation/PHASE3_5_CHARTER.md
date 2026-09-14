# Phase 3.5 — Pre-Build Validation Charter

Status: APPROVED
Owner: Namit Singh
Phase: 3.5 — Pre-Build Validation
Basis: Phase 1 fb5f23f; Phase 2 2f7f09d/9e36d02; **Phase 3 baseline 6ff70ca**.

> **APPROVED — Phase 3.5 validation-design baseline (2026-09-14; DEC-013).** Approval followed owner CONDITIONAL PASS, amendment cycles and a final consistency/terminology cleanup. It authorises this validation protocol as the **current baseline**; it does **NOT** authorise participant execution, the dry run, Track B, Phase 4 or a software build. Phase 3.5 itself is **not** complete (no evidence collected). This charter sets up the Phase 3.5 validation design and governance ONLY. No participant sessions have run; no assumption is validated; no software is built; Phase 4 is not authorised. Synthetic scenarios only — no real/confidential organisation or data.

## 1. Why this phase exists

Phase 3 produced an approved, traceable, implementation-neutral requirements baseline but explicitly did **not** establish that a dedicated custom product is necessary. Before any UX, architecture or build investment, Phase 3.5 seeks **directional real-user evidence** about the BA operating discipline, and then tests whether configurable existing tools would suffice.

## 2. What is being tested

- **ASM-002** — Does the structured BA operating discipline improve the quality, consistency and defensibility of AI-opportunity decisions?
- **ASM-004** — Will intended practitioners use the discipline without disproportionate burden?
- Later (Track B): whether **configurable existing tools** satisfy the approved Phase 3 requirements before any custom-product decision (informs ASM-005 / RSK-001 and the Phase 3 product-necessity conclusion).

## 3. What is explicitly NOT being claimed

- ASM-002 / ASM-004 / ASM-006 / ASM-010 remain **OPEN**; nothing here validates them.
- ASM-010 (enterprise causation) is **out of scope** for a small synthetic pilot — it needs comparative/longitudinal real-world evidence.
- Dedicated custom-product necessity remains **UNPROVEN**.
- Directional validation is **not** statistical proof; synthetic-case performance is **not** enterprise-outcome proof.
- No build, no Phase 4, no UX, no architecture/stack/model/provider, no code.
- The pre-build validation prototype is **not** a software MVP.

## 4. Two-track SEQUENTIAL model

- **Track A — Discipline validation** (first): test the discipline itself, **without custom software and without AI assistance**, to isolate whether the structured discipline creates value (ASM-002/ASM-004).
- **Track B — Existing-tool sufficiency** (only after Track A evidence exists): evaluate whether configurable existing tools provide enough workflow control, hard-gate enforcement, authority separation, traceability, change/reopen behaviour and provenance before concluding a custom product is warranted. Compare the **approved requirements** against what existing tools demonstrably provide — never against a fictional custom product. (Track B execution is not part of this atomic task.)

## 5. GO / MODIFY / STOP decision matrix (pre-committed, qualitative — owner decision after Track A)

This is a **pre-committed qualitative decision matrix**, fixed before any session. It is **not numeric**: no numeric thresholds are used unless the owner explicitly writes and approves them into SCORING_RUBRIC.md §7 beforehand, with justification. The decision is read from the A–F indicator profiles (SCORING_RUBRIC.md) and the **independent hard-blocker flag**, interpreted qualitatively.

| Outcome | Qualitative pattern (read from the rubric, not a score) | What it authorises |
|---|---|---|
| **GO** | Condition B shows a **consistent, visible improvement** in decision-quality behaviours (problem/evidence discipline, non-AI consideration, blocker detection, defensible routing) over credible current practice, **and** blockers are reliably caught, **and** burden appears acceptable relative to the benefit. | Continue the structured discipline / validation. **Track B MAY NOW BE CONSIDERED for separate owner authorisation** — GO itself does **NOT** authorise Track B (Track B has its own owner gate, TRACK_B §0) and does **NOT** authorise a build. |
| **MODIFY** | Some genuine value is visible **but** important friction, gaps, confusion or inconsistent behaviour mean the operating model/prototype must change before proceeding; or burden is high in specific, fixable ways. | Revise the discipline/prototype/protocol and re-test the affected part before advancing. |
| **STOP / RETHINK** | Little or no observable decision-quality improvement over credible current practice; **or** blockers are missed as often as under current practice; **or** disproportionate burden; **or** clear user rejection. | Do not advance toward a product on this basis; rethink the premise. |

Decision rules that override the headline pattern:
- A **missed hard blocker** (rubric C2 = 0 on a blocker scenario) is always surfaced and weighed explicitly; it is never averaged away by good performance elsewhere.
- **GO authorises neither Track B nor a build.** No GO outcome authorises Track B, custom software, UX, architecture, stack, provider or code. Track B requires its own separate owner authorisation (TRACK_B §0); a build requires Track B **and** a further separate owner decision.
- If Track A evidence is **inconclusive** (too few completed sessions, dry-run problems unresolved, matched-pair equivalence in doubt), the default is **MODIFY / re-run**, not GO.

## 6. Governance and constraints

- Synthetic only; never Primark, the owner's employer, or any real confidential organisation/data.
- Existing identifier families only (SCN for scenarios); no new family.
- AI not required for Track A; detailed value measurement not required for Track A.
- Minimal participant data; anonymised (see PARTICIPANT_PLAN.md).
- Repository drafts remain uncommitted/unpushed pending owner review.

## 7. Quality challenge (answered honestly)

| Challenge | Answer / mitigation |
|---|---|
| Are we testing ASM-002, or merely whether users like a template? | Track A compares matched cases with vs without the discipline and scores **observable decision-quality behaviours** (evidence gaps found, non-AI considered, blockers spotted), not just preference. Preference is captured separately as subjective feedback. |
| Does the comparison isolate the discipline from AI/tool effects? | Track A runs **no AI** and **no custom software** — only the discipline vs a lightweight approach. AI/tool effects are deferred (Track B / later). |
| Are scenarios biased to make the structured process win? | Scenarios include cases where the disciplined answer is **non-AI, PARK or STOP**, and a "high headline value behind a blocker" trap; a template that manufactures analysis would score worse, not better. Owner reviews scenarios for bias before testing. |
| Does the rubric reward judgement, not compliance? | The rubric rewards **defensible reasoning** and allows multiple reasonable decisions; it does not reward reaching one prescribed answer or filling every field. |
| Are we creating too much process burden? | NFR-007 (proportionality) is itself under test; the prototype is deliberately lighter than the full Phase 3 catalogue, and burden/time are measured. |
| Could participants infer the desired answer? | Briefing is neutral (see PARTICIPANT_PLAN.md); counterbalanced order; facilitator avoids leading; the "AI because AI" trap detects acquiescence. |
| Are we treating synthetic performance as enterprise proof? | No — explicitly directional; ASM-010 stays OPEN; results will say "directional, synthetic, not enterprise proof". |
| Could a much simpler checklist achieve the same improvement? | A valid **possible finding / future-simplification option**, not something built into the study: "a lighter checklist would suffice" is an accepted, non-failure outcome. It is **not** wired into Condition A — Condition A stays **credible current practice** (natural approach / ordinary notes / lightweight unstructured worksheet), never a Phase 3.5-designed checklist, unless a checklist genuinely is a given participant's own pre-existing method. |
| Does Track B genuinely challenge custom-product necessity? | Track B scores existing tools against the **approved requirements**, not against a strawman; "existing tools suffice" is an accepted outcome. |
| What evidence would make us STOP rather than rationalise a build? | Defined in the GO/MODIFY/STOP matrix and rubric: little decision-quality improvement, blockers missed as often as current practice, disproportionate burden, user rejection, or Track B showing existing tools suffice. |
| Is Condition A a fair baseline, or a strawman set up to lose? | Condition A is **credible current practice** — a competent practitioner's natural/lightweight approach on a **matched case of comparable difficulty** (not a blank page, not an impoverished one). Its scenario's information set is fixed independently of condition, so a Condition B "win" cannot be an artefact of a weaker baseline. (VALIDATION_PLAN §2.) |
| Is the *only* difference between conditions the discipline (not more info or better tooling)? | Yes by design: each scenario's information set is **fixed independently of the condition it is assigned to**; A and B use **matched-but-different** scenarios of comparable information quantity, quality, ambiguity and difficulty (facts **not literally identical**); **neither condition receives privileged/additional evidence** because of its condition; Condition B differs through **structure**, not better information or tooling, and adds **no configured workflow software**. Tool effects are deferred to Track B. (VALIDATION_PLAN §2, §10.) |
| Could a learning effect inflate the later condition? | Recognised risk: AB/BA counterbalancing distributes it; matched-but-different cases reduce direct carryover; the residual learning/carryover risk is **recorded and factored into interpretation**, not ignored. (VALIDATION_PLAN §2.1.) |
| Is the sample big enough to prove anything? | No — 6–8 completed participants is a **practical directional target**, not a statistically justified sample. Results are directional; ASM-002/004 remain OPEN. (PARTICIPANT_PLAN §2.) |
| Does the scoring hide failures behind a good average? | No composite score exists. Indicators are reported as **per-dimension profiles**, and a **missed hard blocker is flagged independently** and never averaged away. (SCORING_RUBRIC §3–§4.) |
| Who decides the outcome, and is it pre-committed? | The **owner** decides against a **pre-committed qualitative** GO/MODIFY/STOP matrix (§5) fixed before testing; GO explicitly does not authorise a build. |

## 7a. Owner questions resolved (Phase 3.5 CONDITIONAL PASS)

Recorded so the design decisions are not re-litigated:
- **Participant target** — RESOLVED: **6–8 completed** participants; **majority practising / BA-heavy**; adjacent roles supplement, do not dominate (PARTICIPANT_PLAN §1–§2).
- **Numeric GO/MODIFY/STOP thresholds** — RESOLVED: **NO numeric thresholds** by default; decision is a pre-committed **qualitative** matrix (§5; SCORING_RUBRIC §7).
- **Condition A** — RESOLVED: **credible current practice, not a blank page/strawman**; A and B use **matched-but-different** scenarios of comparable difficulty (each scenario's information set fixed independently of condition; no privileged evidence either side; Condition B differs through structure, not information/tooling) (VALIDATION_PLAN §2).
- **Track A tooling** — RESOLVED: **lightweight structured document/worksheet only**; no configured Jira/Notion workflow (that is Track B) (VALIDATION_PROTOTYPE_SPEC §1–§2).
- **Scenario load** — RESOLVED: **~2 matched pairs = ~4 cases** per participant, drawn/rotated from a broader SCN bank, matched and matching-reviewed (VALIDATION_PLAN §3, §5; SCENARIO_PLAN).

## 8. Artefacts (all DRAFT; execution NOT STARTED)

docs/validation/: PHASE3_5_CHARTER.md (this) · VALIDATION_PLAN.md · VALIDATION_PROTOTYPE_SPEC.md · SCENARIO_PLAN.md · SCORING_RUBRIC.md · PARTICIPANT_PLAN.md · TRACK_B_TOOL_EVALUATION_PLAN.md. Private evidence register: evidence/PHASE_03_5_EVIDENCE.md. No RESULTS/SYNTHESIS artefacts exist yet — Track A and Track B are **NOT STARTED**.
