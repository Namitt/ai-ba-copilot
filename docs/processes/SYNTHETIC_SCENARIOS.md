# Phase 2 Synthetic Stakeholder Scenarios

Status: APPROVED
Owner: Namit Singh
Phase: 2 — BA Operating Model & Business Process
Date: 2026-09-11
Baseline: Phase 1 content fb5f23f; closure 3cdbcce.

> Owner-approved as part of the Phase 2 BA operating-model baseline on 2026-09-11 (content commit 2f7f09d). Approval accepts these scenarios as the project's synthetic test set for internal stress testing; it does not make them empirical evidence, and prevalence, causation and efficacy remain unestablished.

**SYNTHETIC SCENARIOS — Not based on a real organisation's confidential/internal information.** All people, records, quantities and constraints below are invented test inputs, not observations, interviews, empirical evidence or forecasts. No application data or code is generated.

## Method and identifiers

These input cases are specified before the process walk-through. Outputs and route judgements are recorded separately in PHASE2_SYNTHESIS.md. Each case deliberately contains evidence that could favour an alternative conclusion. SCN-001..004 are local scenario identifiers; SCN-001/E1 means an invented evidence premise, never an external EV source. Existing PP, ASM, RSK and STK identifiers are retained without renumbering. No real interview was held. Stakeholder concerns are authored role perspectives, not quotations from people.

## SCN-001 — Support query routing

**SYNTHETIC SCENARIO — Not based on a real organisation's confidential/internal information.**

- Original request: “Can AI route incoming support messages so customers reach the right team sooner?”
- Context/requestor: hypothetical service operation; STK-01 service manager owns the problem. STK-02 BA coordinates discovery; STK-03 innovation sponsor; STK-04 engineering; STK-05 finance; STK-06 privacy; STK-07 delivery; STK-08 agents and customers participate.
- Pain: avoidable transfers delay resolution; manual first sorting competes with complex case work. A proposed AI tool is not yet an evidenced remedy.
- Known invented evidence: E1 a four-week queue summary has 2,000 messages and 360 transfers; E2 an invented 100-message sample attributes 12 transfers to ambiguous category rules and six to free-text interpretation; E3 routing activity totals an assumed 100 staff-hours in that period. The small sample is not representative of the full queue; transfers are not all errors.
- Missing evidence: independent route labels, urgency and language coverage, seasonal variation, first-contact resolution, customer waiting time, privacy review and actual avoidable handling time.
- Current state: an agent reads the message, chooses a team and records a category; a receiving team may transfer it. A category guide and ticket IDs already exist. Capacity and queue ownership also affect waiting time.
- Available data/limitations: hypothetical timestamps, categories, transfer events and free text; inconsistent historical labels, duplicate messages and potentially personal data. No data has been accessed. Permission to use any real text is unknown and must not be assumed.
- Dependencies: agreed category ownership, export feasibility, service capacity, routing exceptions and operational manager availability.
- Stakeholder concerns: agents fear loss of discretion and added checking; engineering doubts label quality; customers need urgent cases handled safely; finance distinguishes released capacity from cash savings.
- AI idea: assisted interpretation of ambiguous text with human routing judgement. Non-AI alternatives: repair category guidance, rules for clear categories, standard request forms, staffing/queue changes or do nothing.
- Potential benefit: less avoidable sorting/rework and shorter waiting time; no established cash benefit or ROI. Any time benefit must deduct checking and rework.
- Feasibility: clear categories may need no AI; ambiguous text may benefit from assistance, but no model performance is known.
- Governance/risk: minimise text exposure; clarify processing permissions, escalation and oversight; STK-06 determines assurance needs. The BA cannot authorise data use.
- Adoption/change: co-design category guidance with agents; identify training/support owner and monitor use, overrides and checking burden.
- Unresolved assumptions: ASM-002, ASM-003, ASM-004, ASM-006, ASM-007, ASM-009, ASM-010. A transfer-rate reduction might merely hide misroutes; average time might improve while urgent cases worsen.

## SCN-002 — “AI” purchase-request routing

**SYNTHETIC SCENARIO — Not based on a real organisation's confidential/internal information.**

- Original request: “We need AI to approve and route purchase requests faster.”
- Context/requestor: STK-01 purchasing manager; STK-05 owns financial control, STK-04 assesses rules automation, STK-07 delivery coordinates changes, STK-08 requestors and approvers use the process; STK-03 sponsors prioritisation and STK-06 reviews data/control concerns proportionately.
- Pain: approvals take too long; staff chase missing information.
- Known invented evidence: E1 120 requests in a four-week sample, 40 returned for missing cost centre; E2 60 wait over two business days for an unavailable approver; E3 an approved synthetic routing table covers department and amount, with five exceptional requests requiring judgement. Categories overlap and must not be added as unique cases.
- Missing evidence: time spent chasing, policy ownership, delegation permissions, exception reasons, delay by route, implementation/change cost.
- Current state: spreadsheet/form intake, fixed routing table, email approval and existing decision record. The main delay may be approver availability rather than classification.
- Available data/limitations: hypothetical amount, department, cost centre, submission and approval dates; incomplete return timestamps. Employee details must be minimised. No real records accessed.
- Dependencies: finance approval of policy/delegation and an operational owner for exceptions.
- Stakeholder concerns: finance rejects unauthorised approval; requestors dislike repeated entry; approvers need legitimate delegation; engineering notes a stable rules table already exists.
- AI idea: interpretation/automatic approval. Alternatives: mandatory completeness checks, explicit routing rules, delegated approval coverage, clearer policy or manual process repair. Ambiguous exception narratives could still justify future assistive analysis if material.
- Potential benefit: fewer returns and shorter waits; no quantified value until baseline and costs exist.
- Feasibility: deterministic checks fit clear fields; missing authority cannot be fixed by a model. Five exceptions do not establish demand for an AI product.
- Governance/risk: retain approval authority; verify segregation/control needs with finance; changes to permissions require accountable review.
- Adoption/change: explain policy and delegation; avoid extra forms; measure rework and approver participation.
- Unresolved assumptions: ASM-002, ASM-004, ASM-005, ASM-006, ASM-010. Process changes may solve the problem without new software; approval policy might prove less stable than stipulated.

## SCN-003 — Personal-data-based hardship prioritisation

**SYNTHETIC SCENARIO — Not based on a real organisation's confidential/internal information.**

- Original request: “Use AI to rank hardship assistance applications and automatically reject low-ranked cases to clear the backlog.”
- Context/requestor: STK-01 service owner, with STK-03 sponsor, STK-02 BA, STK-04 technical assessor, STK-05 finance, STK-06 privacy/governance specialists, STK-07 delivery and STK-08 applicants/caseworkers. This is a fictional service, not a real public body or organisation.
- Pain: delayed assistance decisions; administrative effort may compete with case assessment.
- Known invented evidence: E1 300 pending applications at a point in time; E2 prior case notes include financial circumstances and possible health information; E3 the service already has a privacy escalation at intake and named human case decision authority; E4 no fairness analysis or independently checked outcome labels exists.
- Missing evidence: arrival/completion rates, eligibility policy, completeness of historic outcomes, lawful processing assessment, DPIA determination, affected-group impacts, meaningful oversight capacity, explanation/contestability arrangements and benefit baseline.
- Current state: trained caseworkers assess each application against policy, record reasons and allow escalation. Queue age alone does not establish inefficient judgement or justify rejection automation.
- Available data/limitations: hypothetical forms and outcome notes with sensitive context, possible historic bias and incomplete appeal outcomes. No real personal data is used or accessed; historical decisions are not objective truth labels.
- Dependencies: service policy authority, qualified privacy/legal assurance, caseworker capacity, accessible review route and data quality review.
- Stakeholder concerns: applicants fear unfair exclusion; caseworkers fear rubber-stamp review; finance needs cost realism; privacy specialists require a case-specific assessment; sponsor wants delay reduced without transferring harm to applicants.
- AI idea: consequential ranking/rejection. Alternatives: checklist completeness assistance, administrative queue allocation, staffing, clearer policy or manual triage with accountable review.
- Potential benefit: reduced waiting/admin load; potential harm could outweigh efficiency. No numerical benefit or fairness claim established.
- Feasibility: label bias, missing appeal outcomes and review capacity make reliable assessment uncertain. No algorithm or model is selected.
- Governance/risk: record intended decision effect, automation level, sensitive data, affected groups, oversight/contestability and specialist DPIA/processing decisions. Whether processing is lawful or a DPIA is required must be determined by authorised specialists using current rules; this document makes no legal determination.
- Adoption/change: caseworkers need time and authority to challenge; affected people need an accessible route to question outcomes. A nominal human click is not evidence of meaningful oversight.
- Unresolved assumptions: ASM-002, ASM-003, ASM-006, ASM-007, ASM-009, ASM-010. Existing early governance challenges the assumption that governance is always late. A carefully bounded administrative option may remain viable even if the original request cannot proceed.

## SCN-004 — Executive “AI sentiment dashboard”

**SYNTHETIC SCENARIO — Not based on a real organisation's confidential/internal information.**

- Original request: “Give us an AI sentiment dashboard; peers seem to have one.”
- Context/requestor: STK-01 department manager; STK-03 sponsor; STK-08 service users; STK-02 BA; STK-04 engineering; STK-05 finance; STK-06 governance and STK-07 delivery consulted only if there is a decision worth supporting.
- Pain: requestor cannot yet identify a recurring business decision that the dashboard would change.
- Known invented evidence: E1 20 voluntary feedback comments from one event; E2 an existing monthly manual summary has no recorded readership; E3 sponsor has no named operational action owner or committed analysis capacity.
- Missing evidence: target decision, affected population, representative feedback, existing summary usefulness, strategic link and beneficiary.
- Current state: comments summarised manually; no action tracking. A dashboard might increase visibility, or simply duplicate an unused report.
- Available data/limitations: small self-selected text sample, sentiment ambiguity and possible personal details; not representative; no longitudinal baseline.
- Dependencies: business decision owner and evidence that feedback changes action.
- Stakeholder concerns: requestor values visibility; end users want action; finance questions opportunity cost; engineering worries about an unused artefact; privacy questions text reuse.
- AI idea: automated sentiment. Alternatives: define the business question, review existing summary, use a facilitated action meeting or stop reporting with no decision use.
- Potential benefit: unknown; neither cost saving nor strategic value evidenced.
- Feasibility: technical possibility is irrelevant until intended use is clear.
- Governance/risk: personal-data screening still applies if later pursued; no inference about people from a small sample should be endorsed.
- Adoption/change: no nominated user workflow or response owner exists.
- Unresolved assumptions: ASM-002, ASM-004, ASM-005, ASM-006, ASM-010. A recurring decision could emerge on clarification; weak initial evidence does not automatically mean permanent rejection.

## Challenge discipline

The cases do not require particular recommendations. Test alternative explanations, minimum evidence and route reversal conditions separately. Preserve these input premises if the lifecycle changes; record any later scenario revision explicitly. SCN-001's existing category guide, SCN-002's approval audit and SCN-003's early governance are counterexamples to universal failure claims. Owner/practitioner review of realism remains outstanding (ASM-009).
