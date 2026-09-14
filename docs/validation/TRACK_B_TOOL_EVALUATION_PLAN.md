# Track B — Existing-Tool Sufficiency Evaluation Plan

Status: APPROVED
Owner: Namit Singh
Phase: 3.5 — Pre-Build Validation
Basis: approved Phase 3 requirements; MVP_BOUNDARY product-necessity challenge; RSK-001; ASM-005.

> **APPROVED (as a PLAN) — Phase 3.5 validation-design baseline (2026-09-14; DEC-013).** Approval of this plan followed owner CONDITIONAL PASS, amendment cycles and a final consistency/terminology cleanup; it authorises this plan as the current baseline. It does **NOT** authorise Track B execution — Track B requires a separate owner decision after Track A evidence (its own trigger gate, §0) — and does **NOT** authorise Phase 4 or a build. Track B runs **only after** Track A evidence exists and is **NOT STARTED**. No tool is selected; no bake-off is conducted in this atomic task. The question is narrow and honest: **can configurable existing tools satisfy enough of the approved Phase 3 requirements that a custom product is unnecessary?** Compare the approved requirements against what existing tools demonstrably provide — never against a fictional custom product.

## 0. Trigger gate (NOT automatic)

Track B does **not** start automatically when Track A ends. It starts **only** when **both**:
1. Track A evidence exists and has been reviewed against the GO/MODIFY/STOP matrix (PHASE3_5_CHARTER §5); **and**
2. The owner makes a **separate, explicit decision** to run Track B.

A **STOP/RETHINK** outcome from Track A means Track B does **not** run. A **GO** outcome permits — but does not compel — Track B; it is still an owner decision, and it is **not** a build decision. Until that decision is recorded, Track B stays **NOT STARTED**; no tool is selected and no evaluation is performed.

## 1. Purpose

Test the Phase 3 product-necessity conclusion (no capability proven to require a custom build; integration value unproven) against real configurable tools, so a build decision is not made on assumption. Informs ASM-005 and RSK-001.

## 2. Candidate tool classes (not a shortlist, not a winner)

- Workflow / project-management tools (statuses, permissions, transitions)
- Forms / workflow-automation tools
- Knowledge / decision-management tools

Specific products are chosen at execution time with owner input; none selected here.

## 3. Evaluation matrix (against approved Phase 3 requirements)

Each candidate is assessed per criterion as **Native / Configurable / Workaround / Not feasible**, with an evidence note (what was actually configured/observed), plus a burden/complexity note. No magic total.

| Criterion (approved requirement) | Source |
|---|---|
| Hard-gate enforcement (blocker prevents progression) | BRULE-002; FR-012 |
| Value cannot override a hard gate | BRULE-003; FR-018 |
| Authority-based permissions; multiple distinct bounded dispositions | BRULE-011; FR-032; NFR-003 |
| Decision/disposition separation | FR-011/017/020 |
| End-to-end traceability (navigable chain) | BR-006; FR-023 |
| Superseded-record retention | BRULE-010; FR-024 |
| Controlled reopen-on-change | BRULE-008; FR-024 |
| Unknown stays unknown / no auto-fill | BRULE-005; FR-005 |
| AI-output provenance/marking (only if AI later enabled) | BRULE-004; FR-026 (conditional) |
| Operational burden (NFR-007 proportionality) | NFR-007 |
| Configuration complexity / maintainability | NFR-011 |

## 4. Method (when executed)

1. Take the approved requirements as fixed acceptance criteria.
2. Attempt to configure each candidate to meet each criterion (time-boxed).
3. Record Native/Configurable/Workaround/Not-feasible + evidence + burden.
4. Summarise where existing tools suffice, where they need awkward workarounds, and where they genuinely cannot meet an approved requirement.
5. Feed into the Phase 3.5 synthesis and the GO/MODIFY/STOP + product-necessity decision.

## 5. Honest-outcome commitment

"**Existing tools are sufficient**" is a valid, accepted outcome that would count against building a custom product. The evaluation must not be framed to make a custom product win; the strongest custom-product hypothesis (integrated enforced-control + traceability layer) is tested by whether configured tools can or cannot provide that integration acceptably.

## 6. Boundaries

Plan only; not started; no tool selected; no build; no architecture/stack/provider; synthetic requirements/data. Track B execution requires the owner's go-ahead after Track A.
