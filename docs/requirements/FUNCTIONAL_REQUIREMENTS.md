# Functional Requirements

Status: APPROVED
Owner: Namit Singh
Phase: 3 — Product Requirements
Basis: BUSINESS_REQUIREMENTS (BR); STAKEHOLDER_REQUIREMENTS (SR); BA_OPERATING_MODEL; OPPORTUNITY_LIFECYCLE (LC); TO_BE_PROCESS; PRIORITISATION_APPROACH.

> APPROVED — owner-approved as part of the Phase 3 Product Requirements baseline on 2026-09-14, after initial draft, owner CONDITIONAL PASS, amendments and final consistency review. Approval accepts this artefact as the current requirements baseline; it does NOT authorise a software build, Phase 4, or the pre-build validation gate (Phase 3.5). Prior review note: Functional requirements are implementation-neutral ("The product shall…"), testable and atomic where practical. They embed NO technology, provider, UI or data-model choice. **Class** = AI / DET (deterministic software) / HUMAN, per the approved control model. **Validation** = SUPPORTED (traces to approved need) or NEEDS VALIDATION (real-user/necessity check required). Priority is MoSCoW, provisional. A functional requirement describing a capability does not assert that the capability must be custom-built; see MVP_BOUNDARY.md.

## Control-model classification key

- **AI**: the product may use AI to assist (analyse, synthesise, draft, suggest). AI never approves or progresses.
- **DET**: deterministic software owns it (validation rules, calculations, workflow state, identifiers, traceability).
- **HUMAN**: a human performs or decides; software records the act.

Most requirements combine classes; the class column names the controlling responsibility.

## Group A — Capture and framing (LC-001, BACT-001)

| ID | The product shall… | Actor | Class | Human control | Source | Priority | Validation |
|---|---|---|---|---|---|---|---|
| FR-001 | record a request with source/channel, stated problem, requested solution, intended decision/use, and business/operational owner | STK-01/02 | DET+HUMAN | BA records; owner named by human | BR-001, SR-001; LC-001 | MUST | SUPPORTED |
| FR-002 | keep "stated problem" and "requested solution" as distinct recorded fields, and flag when options work proceeds without the distinction recorded | STK-02 | DET | BA resolves the flag | BR-001; PP-002 | MUST | SUPPORTED |
| FR-003 | offer an AI-assisted summary of recorded source material, preserving links to sources and marking the output AI-generated until human review | STK-02 | AI+HUMAN | BA reviews before use | BR-008, SR-001; EV-007 | SHOULD | NEEDS VALIDATION |

## Group B — Evidence (LC-002, BACT-002)

| ID | The product shall… | Actor | Class | Human control | Source | Priority | Validation |
|---|---|---|---|---|---|---|---|
| FR-004 | let evidence be attached to a claim with a reference, or a field be explicitly marked "unknown" | STK-02 | DET | BA judges sufficiency | BR-002, SR-002 | MUST | SUPPORTED |
| FR-005 | never auto-fill or infer an "unknown" as fact (unconditional); and, where AI suggestions exist, keep AI-suggested values visibly distinct from human-confirmed values until a human confirms them | STK-02 | DET (+ AI control when AI enabled) | BA confirms values | BR-002; BRULE-005; RSK-004 | MUST (AI-distinct part CONDITIONAL — IF AI ENABLED) | SUPPORTED |
| FR-006 | surface the unresolved evidence gaps for an opportunity to the BA | STK-02 | DET | BA acts on gaps | BR-002, SR-002 | MUST | SUPPORTED |

## Group C — Options (LC-003, BACT-003)

| ID | The product shall… | Actor | Class | Human control | Source | Priority | Validation |
|---|---|---|---|---|---|---|---|
| FR-007 | let the BA record explicit consideration of AI applicability and compare options — where AI is credible/requested, AI vs credible non-AI and no-change; where AI is not credible, record that conclusion with the non-AI/no-change options (no fictional AI option manufactured) | STK-02/04 | DET+HUMAN | BA/specialists judge | BR-003, SR-003; SCN-002 | MUST | SUPPORTED |
| FR-008 | retain rejected options with their reasons rather than discarding them | STK-02 | DET | — | BR-003; BRULE-010 | MUST | SUPPORTED |
| FR-009 | offer AI-assisted candidate options and objections, marked AI-generated and non-authoritative | STK-02 | AI | BA selects/rejects | BR-008 | COULD | NEEDS VALIDATION |

## Group D — Assurance and governance (LC-004, BACT-004)

| ID | The product shall… | Actor | Class | Human control | Source | Priority | Validation |
|---|---|---|---|---|---|---|---|
| FR-010 | capture governance fields per opportunity early: personal-data use, DPIA trigger, ADM significance/automation level, oversight point, fairness/transparency need, accountable owner | STK-02/06 | DET | specialist interprets | BR-004, SR-008; F-D1 | MUST | SUPPORTED |
| FR-011 | let an accountable specialist record an assurance disposition per option (passed / conditions / blocked) with conditions and scope | STK-06 | HUMAN | specialist decides | BR-004, SR-008; BACT-004 | MUST | SUPPORTED |
| FR-012 | prevent a progression action whose required assurance is unresolved or blocked from being marked progressed | — | DET | specialist clears blocker | BRULE-002 | MUST | SUPPORTED |
| FR-013 | route an early triage governance referral back to discovery/options (never straight to LC-004 assurance), allowing the affected activity to be held while safe analysis continues | STK-02/06 | DET workflow | specialist/BA | TO-BE routing; BRULE-007 | MUST | SUPPORTED |

## Group E — Value and measurement (LC-004/005, BACT-005)

| ID | The product shall… | Actor | Class | Human control | Source | Priority | Validation |
|---|---|---|---|---|---|---|---|
| FR-014 | let a value baseline, period, measurement owner and expected-vs-actual plan be defined for an opportunity | STK-02/05 | DET+HUMAN | finance validates | BR-005, SR-007 | SHOULD | NEEDS VALIDATION |
| FR-015 | perform value/effort arithmetic deterministically with explicit units, period and assumptions; not annualise or monetise without a supported basis | — | DET | BA/finance review | BR-005; PRIORITISATION | SHOULD | SUPPORTED |
| FR-016 | keep "released capacity" distinct from "cash saving" and withhold an ROI conclusion where implementation/operating costs are unknown | — | DET | finance decides | BR-005 | SHOULD | SUPPORTED |

## Group F — Prioritisation and recommendation (LC-005, BACT-006)

| ID | The product shall… | Actor | Class | Human control | Source | Priority | Validation |
|---|---|---|---|---|---|---|---|
| FR-017 | record hard-gate dispositions (permission, decision-owner, funding authority, material assurance) separately from ranking inputs | STK-02/03 | DET | authorities decide gates | BR-007; PRIORITISATION | MUST | SUPPORTED |
| FR-018 | prevent ranking from overriding an unresolved hard gate | — | DET | — | BRULE-003 | MUST | SUPPORTED |
| FR-019 | let a BA record a recommendation with alternative, conditions, confidence and reconsideration trigger, marked as a recommendation not an approval | STK-02 | HUMAN | BA owns; sponsor decides | BR-008, SR-005; LC-005 | MUST | SUPPORTED |

## Group G — Decision and handoff (LC-006, BACT-007)

| ID | The product shall… | Actor | Class | Human control | Source | Priority | Validation |
|---|---|---|---|---|---|---|---|
| FR-020 | let an accountable authority record a decision (proceed / non-AI route / refine / more-evidence / park / stop) with rationale, conditions, reviewer, date | authorities | HUMAN | authority decides | BR-009; LC-006 | MUST | SUPPORTED |
| FR-021 | require a park to retain a revisit trigger and a stop to retain a reason; neither deletes the record | — | DET | — | BRULE-006 | MUST | SUPPORTED |
| FR-022 | record a receiving owner on a proceed decision, and a measurement owner only where value measurement is part of the authorised next action (otherwise preserve the measurement gap/condition explicitly) | STK-07/01 | DET+HUMAN | owners accept | BR-006, SR-009 | SHOULD | SUPPORTED |

## Group H — Traceability and change

| ID | The product shall… | Actor | Class | Human control | Source | Priority | Validation |
|---|---|---|---|---|---|---|---|
| FR-023 | maintain a navigable chain from decision back to request, evidence, assumptions, options, assurance, value basis and accountable authorities | — | DET | — | BR-006 | MUST | SUPPORTED |
| FR-024 | reopen the relevant decision gate when purpose, data, decision effect, cost or ownership materially changes, retaining superseded records | STK-02 | DET rule | BA/authority | BRULE-008/010 | MUST | SUPPORTED |
| FR-025 | record, per bounded decision or disposition, the single accountable authority and any dissent | authorities | DET+HUMAN | — | BR-006; BRULE-009/011 | MUST | SUPPORTED |

## Group I — AI-assist controls (capability/control level, provider-neutral)

> Applicability: FR-026..029 and NFR-002 are **CONDITIONAL MUST — IF AI ENABLED**. They are mandatory whenever AI capability is included in a build, but the pre-build validation prototype is not required to include AI, so their presence is not proof that AI must be in the first prototype. FR-003 and FR-009 (AI conveniences) remain SHOULD/COULD and NEEDS VALIDATION.

| ID | The product shall… | Actor | Class | Human control | Source | Priority | Validation |
|---|---|---|---|---|---|---|---|
| FR-026 | mark all AI-generated content as AI-generated and unreviewed until a human reviews it, and never treat AI output as an approval | — | AI control | human review gate | BR-008; BRULE-004 | CONDITIONAL MUST — IF AI ENABLED | SUPPORTED |
| FR-027 | keep AI summaries source-grounded, preserving links to the supplied source material | — | AI control | — | EV-007 | CONDITIONAL MUST — IF AI ENABLED | SUPPORTED |
| FR-028 | let a human edit, reject or correct any AI output, retaining the change | STK-02 | HUMAN | — | BR-008 | CONDITIONAL MUST — IF AI ENABLED | SUPPORTED |
| FR-029 | represent AI uncertainty rather than fabricating a value, and continue the workflow safely if the AI capability is unavailable or rate-limited | — | AI control | BA proceeds manually | RSK-004; EV-011 (op-cost) | CONDITIONAL MUST — IF AI ENABLED | SUPPORTED |
| FR-030 | not depend on a single AI provider for workflow state, treating provider/model choice as an external, deferrable decision | — | DET | — | DEC-003; ASM-008 | SHOULD | SUPPORTED |
| FR-031 | keep an audit trail that AI assistance was used and on what source, without embedding a provider choice | — | DET | — | BR-006 | SHOULD | SUPPORTED |

## Group J — Access and authority

| ID | The product shall… | Actor | Class | Human control | Source | Priority | Validation |
|---|---|---|---|---|---|---|---|
| FR-032 | permit an action only to a role with the legitimate authority for it (assurance disposition → accountable specialist; spend disposition → funding authority; decision → accountable authority) | all | DET | — | RACI; NFR-003; BRULE-011 | MUST | SUPPORTED |

## Cross-cutting human-control note

FR-012, FR-018, FR-021 and FR-026 together encode the non-negotiable controls: AI cannot approve (FR-026, whenever AI is enabled); unknowns cannot become fact; blocked/parked/stopped opportunities cannot silently progress; and a high score cannot offset a hard gate. FR-012/018/021 are MUST regardless of AI; FR-026 is CONDITIONAL MUST — IF AI ENABLED. All derive from locked principles (DEC-002) and approved rules, not hypotheses.

## Requirements flagged NEEDS VALIDATION

FR-003, FR-009, FR-014 (and, at capability level, most AI-assist niceties) are genuinely useful but their necessity for a build is unproven; they must not silently become MUST. FR-009 and FR-003 are AI conveniences; FR-014 depends on ASM-006 (baselines obtainable — OPEN).

## Open questions (functional level)

- OQ-F1: RESOLVED (owner) — AI-assist (FR-003/009) is NOT required for the pre-build validation prototype; the discipline is tested with deterministic capture + human analysis. AI controls (FR-026..029) apply only if AI is enabled.
- OQ-F2: Does FR-013's routing need software, or is it a process rule enforceable in Jira/Notion states?
- OQ-F3: RESOLVED (owner) — measurement (FR-014..016) is SHOULD and excluded from the pre-build validation prototype; ASM-003/ASM-006 remain OPEN.
