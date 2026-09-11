# BA Operating Model

Status: DRAFT
Owner: Namit Singh
Phase: 2
Basis: approved Phase 1 at fb5f23f / 3cdbcce; OPPORTUNITY_LIFECYCLE.md; processes/SYNTHETIC_SCENARIOS.md.

## Boundary and operating stance

The BA enables an accountable recommendation, not universal approval. This is a tailored project interpretation of BA practice informed by the existing EV-007/EV-018 records and Phase 1 findings, not a claim that a professional framework mandates this sequence. Activities can overlap and recur. No new external research was used. No detailed requirements, acceptance criteria, UI or architecture are specified.

Common record discipline: retain original request, scenario/evidence premise or external source, interpretation, uncertainty, author/reviewer, decision authority and next action. Source claims remain distinct from project judgement. AI text remains DRAFT until owner review; a completeness check cannot confer substantive approval. Existing records may be referenced rather than copied.

## BACT-001 — Plan and triage proportionately (LC-001)

- Purpose/decision: spend analysis effort only on a defined question; choose depth, participants and urgent referral.
- Inputs/information: request, business owner, intended use, affected people, existing references, sensitivity, urgency and known constraints.
- BA activity/techniques: clarify need versus requested solution; scope boundary; stakeholder analysis; document review; risk-oriented elicitation planning. Plan interviews/workshops only for later authorised real engagement; none conducted here.
- Participants: STK-01/02/03; STK-06 for risk flags and STK-08 for work impact.
- AI assistance: summarise request, suggest missing questions and possible alternative interpretations; never assert invented answers.
- Deterministic support: detect missing mandatory identifiers/owners; duplicate-reference checks; record dates and workflow disposition. Unknown remains unknown.
- Human judgement: BA assesses relevance and proportionality; sponsor allocates capacity; specialist determines assurance route.
- Output/traceability: bounded analysis plan and triage record linked to request/SCN, stakeholder and initial ASM/RSK references.
- Exit/next routes: LC-001 evidence minimum met, or documented REFINE/MORE EVIDENCE/PARK/STOP/ESCALATE route. Avoid full analysis for SCN-004 without a decision use.

## BACT-002 — Understand problem and evidence (LC-002)

- Purpose/decision: determine whether the stated problem and causal explanation are credible enough for options analysis.
- Inputs/information: triage, current process, baseline definition/period/denominator, exceptions, evidence provenance and missing data.
- BA activity/techniques: process mapping, document/data review, root-cause questioning, observation plan, stakeholder mapping and assumption analysis. Compare alternative explanations rather than declaring a cause from correlation.
- Participants: STK-01/02/08, engineering for data feasibility, finance for measurement validity, governance for permitted evidence use.
- AI assistance: group reported concerns, draft process narrative, surface contradictory premises and unanswered questions; BA checks each against evidence.
- Deterministic support: arithmetic, denominator/period checks, detect duplicate counts, label missing values. Do not infer causation or convert missing data to zero.
- Human judgement: business owner confirms context, users challenge work reality, BA qualifies evidence and tests explanations.
- Output/traceability: problem/evidence/gap record, current-state and stakeholder references, PP/ASM links. Preserve Phase 1 baseline instead of rewriting hypotheses as facts.
- Exit/next routes: LC-002 criteria; LC-003, targeted evidence collection, refinement, park/stop or specialist escalation. SCN-002 overlap in delay counts prevents false totals.

## BACT-003 — Develop and challenge options (LC-003)

- Purpose/decision: identify plausible interventions addressing the need, including no change and non-AI solutions.
- Inputs/information: problem/evidence record, existing controls/tools, constraints, potential harms, current capability and dependencies.
- BA activity/techniques: options analysis, facilitated challenge, process simplification and decision analysis. Compare manual improvement, explicit rules, existing tools and assistive AI without choosing implementation technology.
- Participants: STK-01/02/04/08 with finance, governance and delivery as needed.
- AI assistance: generate alternative options and objections; distinguish suggestions from sourced capability claims.
- Deterministic support: compare documented criteria, track missing assessments and option-to-problem links.
- Human judgement: BA tests need-fit, business owner/user assess usefulness, technical specialist judges plausibility; no AI-selected winner.
- Output/traceability: shortlist and rejected options with evidence/assumptions, harms, reasons and conditional routes.
- Exit/next routes: credible non-AI/do-nothing comparison present; LC-004, refine or seek evidence; sponsor may park/stop. SCN-002 favours rules/process repair but exceptions keep AI assistance a future possibility.

## BACT-004 — Integrate specialist assurance and feasibility (LC-004)

- Purpose/decision: establish what may responsibly be investigated or progressed and which conditions block it.
- Inputs/information: shortlist, data origin/use/access, intended decision effects, technical dependencies, oversight capacity and organisational delegation.
- BA activity/techniques: risk analysis, responsibility mapping, dependency analysis, structured specialist review and unresolved-question tracking.
- Participants: STK-04 technical authority; STK-06 data/privacy/governance authority; STK-01 business owner; STK-07 receiving delivery owner; BA coordinates.
- AI assistance: draft questions, collate supplied assurance findings, surface inconsistencies; never issue legal clearance or technical sign-off.
- Deterministic support: check whether required specialist disposition/reference exists and whether conditions are unresolved; track review triggers. A blank assurance field is not approval.
- Human judgement: relevant specialists determine feasibility and the applicable assurance constraints and blockers. Within those constraints, the appropriately delegated business/sponsor authority decides whether to accept residual business/operational risk and whether the opportunity remains worth pursuing; that authority cannot override a legal, policy, privacy or specialist hard blocker. BA cannot override a blocker by scoring value highly.
- Output/traceability: per-option assurance/feasibility disposition linked to evidence and named authority, with scope, conditions and re-review trigger.
- Exit/next routes: LC-004 criteria, or MORE EVIDENCE/ESCALATE/REFINE/PARK/STOP. SCN-003 remains held for the consequential automation proposal; safer administrative alternatives can be separately assessed.

## BACT-005 — Frame value, adoption and measurement (LC-004)

- Purpose/decision: decide whether expected benefit justifies further effort and how later results could be judged.
- Inputs/information: baseline, volume, time/cost drivers, beneficiaries, harms, costs, capacity constraints and change owner.
- BA activity/techniques: benefits mapping, cost-benefit reasoning, sensitivity analysis, change-impact analysis and measurement planning. Tailor technical/use/operational/strategic/financial layers from existing EV-012; do not assume deployment equals value.
- Participants: STK-01 owns operations/benefit realisation under delegation; STK-05 validates finances; STK-08 assesses work impact; STK-04/07 assess effort; STK-02 integrates.
- AI assistance: draft benefit chains and omitted-cost questions; no fabricated metric values.
- Deterministic support: reproducible arithmetic with explicit units, period, assumptions and uncertainty. Capacity released is separate from cash savings; avoid double-counting.
- Human judgement: finance validates conversion to money; operational owner judges practical capacity use and change readiness; BA tests causal chain and measurement gaps.
- Output/traceability: baseline-to-expected-to-later-actual measurement plan, owner/data source/frequency, cost and adoption dependencies linked to option and recommendation. No actual pilot measures asserted.
- Exit/next routes: decision has proportionate benefit evidence or explicitly recommends bounded validation; LC-005 or refine/evidence/park. SCN-001 cannot claim positive ROI while review/rework costs are unknown.

## BACT-006 — Compare priorities and recommend (LC-005)

- Purpose/decision: recommend the next action using transparent trade-offs rather than a universal score.
- Inputs/information: eligible options, hard gates, confidence, value, strategy, feasibility, effort, adoption, dependency and capacity.
- BA activity/techniques: decision table, pairwise comparison when comparable, sensitivity testing and dissent capture. Use PRIORITISATION_APPROACH.md; do not invent a portfolio optimum from four authored cases.
- Participants: BA, sponsor, business owner, finance, engineering, governance and delivery.
- AI assistance: draft comparison narrative and strongest objection; BA checks completeness and bias.
- Deterministic support: filter documented gate dispositions, normalise units where legitimate, calculate explicit scenarios; no hidden weights.
- Human judgement: BA owns recommendation quality; sponsor owns portfolio priority; finance/spend and assurance decisions remain separate.
- Output/traceability: evidence-backed recommendation, alternative rejected, uncertainty, requested decision and reconsideration trigger.
- Exit/next routes: LC-005 criteria; decision handoff, targeted evidence, refinement or park. High potential value cannot cancel a hard gate.

## BACT-007 — Secure decision and transfer accountability (LC-006)

- Purpose/decision: record what was actually authorised, who receives the next work and how learning returns.
- Inputs/information: recommendation, specialist conditions, decision authorities, unresolved questions and measurement/change plan.
- BA activity/techniques: decision review facilitation, traceability review and handoff walkthrough. Record dissent and conditions rather than smoothing away conflict.
- Participants: STK-03, relevant STK-01/04/05/06/07 authorities and STK-02; affected users consulted proportionately.
- AI assistance: draft decision/handoff summary from recorded decisions; never generate signatures or approval claims.
- Deterministic support: record disposition/time/version, condition ownership and review date/event; retain history on reopening.
- Human judgement: authorised humans decide; receiving owner accepts next work; project owner reviews and approves substantive project drafts.
- Output/traceability: request → evidence/assumptions → options → assurance/value → recommendation → decision → receiving/measurement owner. Later requirements/pilot references are pending future authorisation, not invented now.
- Exit/next routes: acknowledged, bounded disposition under LC-006; otherwise pending decision. PROCEED/NON-AI/PARK/STOP/REFINE/evidence/escalation as appropriate. No automatic entry into Phase 3.

## Proportionality and quality challenge

Use existing finance approvals, ticket references or governance records when adequate. SCN-002 may require a short evidence/decision record, while SCN-003 needs multiple specialists. Measure analysis burden as a future validation question: extra documentation may reduce adoption without improving decisions (ASM-002/004). The process proposal is not proof a dedicated application is necessary.
