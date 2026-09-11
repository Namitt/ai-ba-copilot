# Phase 1 Discovery — Source Register

Status: APPROVED
Owner: Namit Singh
Last Updated: 2026-09-11
Phase: 1 — Formal Discovery & Business Case (owner-approved baseline)

> Owner-approved as the Phase 1 discovery baseline on 2026-09-11 (baseline commit fb5f23f). Approval accepts this source register as the current baseline; source limitations recorded per entry stand.

## Purpose

Traceable register of external sources used in Phase 1 discovery. Each source is classified by type. Vendor material is labelled as vendor claim and is not treated as neutral evidence. Access date for all entries: 2026-09-11.

Source-type key: LAW/REG (statute or regulator guidance), GOV-POLICY (non-statutory government policy framework), GOV-PRACTICE (government practice guidance, not law for private organisations), ANALYST (analyst/research firm survey), PROF-BODY (professional body), INDUSTRY (industry/academic-affiliated report), VENDOR (vendor product/marketing), SECONDARY (secondary analysis).

Verification key for figures: each figure below was checked against the cited source on the access date.

---

### EV-001 — Gartner: forecast that 30% of GenAI projects abandoned after PoC
- Organisation/author: Gartner (Rita Sallam, Distinguished VP Analyst)
- Type: ANALYST
- URL: https://www.gartner.com/en/newsroom/press-releases/2024-07-29-gartner-predicts-30-percent-of-generative-ai-projects-will-be-abandoned-after-proof-of-concept-by-end-of-2025
- Published: 2024-07-29 | Accessed: 2026-09-11
- Key finding: This is a **forecast/prediction**, not an observed rate — Gartner *predicts* at least 30% of generative-AI projects will be abandoned after proof of concept by end of 2025. Cited causes: poor data quality, inadequate risk controls, escalating costs, unclear business value.
- Relevance: Shows that unclear value, data quality, risk controls and cost are cited as factors associated with potential post-PoC abandonment; relevant to the criteria used when assessing opportunities.
- Limitations: A prediction, not a measured outcome; press-release summary of paywalled research. Must not be cited as a measured 30% failure rate.

### EV-002 — MIT NANDA: The GenAI Divide — State of AI in Business 2025 (preliminary)
- Organisation/author: MIT NANDA (Project NANDA)
- Type: INDUSTRY (academic-affiliated; **preliminary findings, not peer-reviewed**)
- URL: https://mlq.ai/media/quarterly_decks/v0.1_State_of_AI_in_Business_2025_Report.pdf (v0.1 report; widely reported via Fortune, Aug 2025)
- Published: July 2025 (research period Jan–Jun 2025) | Accessed: 2026-09-11
- Methodology (verified against the report): 300+ publicly disclosed AI initiatives reviewed; 52 structured organisational interviews; 153 senior-leader survey responses (collected at four industry conferences).
- Precise claim (verified): "95% of organizations are getting zero return" / no measurable P&L impact, while ~5% of integrated pilots extract significant value. Separately: of enterprise-grade custom tools, ~60% evaluated, ~20% reached pilot, ~5% reached production.
- **Do not restate as "95% of AI projects fail."** The claim is about organisations seeing no measurable P&L return, not universal project failure.
- Relevance: Evidence of a large gap between AI activity and measured financial value; points to integration/adoption, not model quality.
- Limitations: Preliminary (v0.1); not peer-reviewed; survey partly convenience-sampled at conferences; "return" defined narrowly.

### EV-003 — McKinsey: The state of AI in early 2024 (historical baseline)
- Organisation/author: McKinsey & Company (QuantumBlack)
- Type: ANALYST (survey) — **historical; retained for comparison, superseded by EV-011/EV-012**
- URL: https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai-2024
- Published: 2024-05-30 | Accessed: 2026-09-11
- Key finding: 65% of organisations regularly used gen AI in ≥1 function; ~72% reported AI adoption overall; value capture early; only ~18% reported enterprise-wide responsible-AI governance.
- Relevance: 2024 baseline for adoption/value trajectory; use only with a clear date label alongside the 2026 evidence.
- Limitations: Now over two years old for a Sept 2026 project; self-reported survey.

### EV-004 — ICO: Guidance on AI and data protection
- Organisation/author: Information Commissioner's Office (ICO), UK
- Type: LAW/REG (regulator guidance)
- URL: https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/artificial-intelligence/guidance-on-ai-and-data-protection/
- Published/updated: originally 2023-03-15; being updated to reflect the DUAA 2025 (see EV-013) | Accessed: 2026-09-11
- Key finding: Applies UK GDPR principles to AI — lawfulness, fairness, transparency, accuracy, accountability/governance — with DPIA considerations and safeguards for solely automated decisions (Article 22).
- Relevance: Governance information a UK AI workflow should capture.
- Limitations: Read together with the DUAA 2025 changes (EV-013), which alter parts of the automated-decision regime.

### EV-005 — ICO: Data Protection Impact Assessments (DPIAs)
- Organisation/author: ICO, UK
- Type: LAW/REG
- URL: https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/accountability-and-governance/data-protection-impact-assessments-dpias/
- Accessed: 2026-09-11
- Key finding: A DPIA is legally required where processing is "likely to result in high risk" — triggers include innovative technologies, large-scale processing, automated decision-making with significant effects, and processing of vulnerable individuals.
- Relevance: When the workflow must prompt a DPIA and what it records.
- Limitations: Criteria-based; case-by-case judgement.

### EV-006 — UK DSIT: A pro-innovation approach to AI regulation (white paper)
- Organisation/author: Department for Science, Innovation and Technology (DSIT), UK
- Type: GOV-POLICY (non-statutory policy framework)
- URL: https://www.gov.uk/government/publications/ai-regulation-a-pro-innovation-approach/white-paper
- Published: 2023-03-29 | Accessed: 2026-09-11
- Key finding: Five cross-sectoral principles — safety/security/robustness; transparency/explainability; fairness; accountability/governance; contestability/redress.
- Relevance: Recognised UK framing for responsible-AI fields.
- Limitations: Principles-based, non-statutory; policy has continued to evolve.

### EV-007 — IIBA: How AI enhances business analysis without replacing judgment
- Organisation/author: IIBA (Stacie A. Benson)
- Type: PROF-BODY (blog/opinion)
- URL: https://www.iiba.org/business-analysis-blogs/how-ai-enhances-business-analysis-without-replacing-professional-judgment/
- Published: 2026-03-11 | Accessed: 2026-09-11
- Key finding: AI accelerates synthesis/admin; BA judgement (technique selection, validation, accountability) stays human — "assistant, not authority."
- Relevance: Professional-body support for the AI-assists/BA-decides control model.
- Limitations: One practitioner's opinion piece, not empirical.

### EV-008 — ITONICS: AI innovation management tools (competitor landscape)
- Organisation/author: ITONICS (vendor)
- Type: VENDOR (claims; partially verified via vendor blog)
- URL: https://www.itonics-innovation.com/blog/ai-innovation-management-tools
- Accessed: 2026-09-11
- Key finding (vendor claim): Innovation-management tooling spans foresight, ideation and portfolio; named platforms include ITONICS, HYPE, Qmarkets, Brightidea, Planview IdeaPlace.
- Relevance: Adjacent innovation-management category.
- Limitations: Vendor marketing; self-described.

### EV-009 — Gartner: AI use-case prioritisation / portfolio offerings
- Organisation/author: Gartner (analyst)
- Type: ANALYST (title/abstract only; paywalled)
- URL: https://www.gartner.com/en/products/ai-use-case-insights ; https://www.gartner.com/en/documents/6663634
- Accessed: 2026-09-11
- Key finding: Gartner offers AI use-case prioritisation/portfolio guidance ("vet, prioritise, fund AI use cases").
- Relevance: Analyst-grade prioritisation already exists (overlap).
- Limitations: Full content paywalled; detail indicative only.

### EV-010 — Practitioner AI use-case prioritisation frameworks (value–feasibility)
- Organisation/author: Multiple practitioner sources
- Type: SECONDARY
- URL: https://enterpriseaiexecutive.ai/p/12-ai-use-case-prioritization-frameworks ; https://iternal.ai/ai-use-case-identification
- Accessed: 2026-09-11
- Key finding: Value-vs-feasibility scoring is a common, widely-repeated prioritisation approach across the reviewed sources.
- Limitations: Secondary/practitioner blogs; convergent but individually non-authoritative.

### EV-011 — McKinsey: The state of AI in 2026 — On the road to ROI
- Organisation/author: McKinsey & Company (QuantumBlack)
- Type: ANALYST (survey) — **current primary adoption/value evidence**
- URL: https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai
- Published: 2026-08-25 | Accessed: 2026-09-11
- Key finding (verified): nearly nine in ten respondents report regular AI use in ≥1 business function; 44% report scaling AI across the enterprise (up from 38% the prior year); 37% report AI has contributed positively to EBIT (essentially unchanged from 2025); ~1 in 5 say their organisation is limiting AI use because of operating costs.
- Relevance: Current adoption-vs-value picture — adoption high, enterprise-scaling and EBIT contribution far lower; cost now a constraint.
- Limitations: Self-reported survey; EBIT contribution is respondent-attributed, not audited.

### EV-012 — McKinsey: From promise to impact — measuring and realising AI value
- Organisation/author: McKinsey & Company (QuantumBlack)
- Type: ANALYST
- URL: https://www.mckinsey.com/capabilities/quantumblack/our-insights/from-promise-to-impact-how-companies-can-measure-and-realize-the-full-value-of-ai
- Published: 2026-04-24 | Accessed: 2026-09-11
- Key finding (verified): ~80% deploy gen AI across functions yet ~60% report no enterprise-wide EBIT impact; proposes a five-layer measurement framework (technical performance → user adoption → operational KPIs → strategic outcomes → financial impact); success comes from measurement built into rollout, a governance cadence with decision gates, shared evidence packs, and staged phases.
- Relevance: Directly supports the deployed ≠ adopted ≠ value model and a concrete measurement method.
- Limitations: Consultancy framework; illustrative rather than independently benchmarked.

### EV-013 — ICO: Data (Use and Access) Act 2025 — what it means for organisations
- Organisation/author: ICO, UK
- Type: LAW/REG (statute + regulator guidance) — **current UK position**
- URL: https://ico.org.uk/about-the-ico/what-we-do/legislation-we-cover/data-use-and-access-act-2025/the-data-use-and-access-act-2025-what-does-it-mean-for-organisations/
- Published/updated: DUAA 2025; data-protection provisions in force by 2026-06-19 | Accessed: 2026-09-11
- Key finding (verified): DUAA 2025 amends UK data-protection law. For automated decision-making it expands the lawful bases available for significant automated decisions (e.g. legitimate interests) provided appropriate safeguards apply — but not for special category data. Also: research provisions, recognised legitimate interests, cookies changes, mandatory complaint procedures. ICO is issuing new/updated guidance.
- Relevance: Refreshes the governance evidence to the Sept 2026 position; the workflow should reflect DUAA-era ADM safeguards.
- Limitations: Some ICO guidance still in draft/rolling out; not legal advice.

### EV-014 — UK Government: Artificial Intelligence Playbook for the UK Government
- Organisation/author: Government Digital Service (GDS), UK
- Type: GOV-PRACTICE (practical guidance for government/public sector — **not law, and not a legal obligation for private organisations**)
- URL: https://assets.publishing.service.gov.uk/media/67aca2f7e400ae62338324bd/AI_Playbook_for_the_UK_Government__12_02_.pdf
- Published: 2025-02 | Accessed: 2026-09-11
- Key finding (verified): Ten principles, including — know AI and its limitations; use lawfully/ethically/responsibly; use securely; **meaningful human control at the right stages**; **manage the full AI lifecycle**; **use the right tool for the job**; be open/collaborative; **work with commercial colleagues from the start**; have the necessary skills; **use principles with organisational policies and assurance**.
- Relevance: Practical, government-tested articulation of human control, lifecycle, right-tool, assurance and commercial involvement — useful design input for what the workflow captures.
- Limitations: Government practice guidance; does not create legal obligations for private organisations; cite as practice, not law.

### EV-015 — IBM Txture: AI transformation planning & assessment (competitor)
- Organisation/author: IBM (vendor)
- Type: VENDOR (verified via product page)
- URL: https://www.ibm.com/products/txture/ai-transformation
- Accessed: 2026-09-11
- Key finding (verified from product page): Assesses the IT/application landscape (ingests CMDB/EA/discovery data), identifies and matches AI use cases via a "5A" method (automate/assist/augment/adapt/autonomize), segments into quick wins/strategic bets and delivery waves, and quantifies effort, cost, payback and multi-year benefit.
- Relevance: Closest to "AI opportunity/transformation assessment," but IT/application-portfolio-centric.
- Limitations: The reviewed product page did not evidence business pain-point discovery, responsible-AI governance capture, requirements or adoption measurement; it is focused on IT/application transformation. (Vendor page — absence of evidence in the reviewed source, not proof of absence.)

### EV-016 — Planview: Strategic Portfolio Management (competitor)
- Organisation/author: Planview (vendor)
- Type: VENDOR (verified via product page)
- URL: https://www.planview.com/products/strategic-portfolio-management/
- Accessed: 2026-09-11
- Key finding (verified): Demand intake (unstructured ideas → formal requests), investment prioritisation (what-if scenarios/business drivers), funding/roadmaps, delivery tracking, and investment-to-outcome/benefits/ROI tracking; AI features for insights/scenario planning.
- Relevance: Serious SPM/PPM covering intake→prioritise→fund→track→benefits.
- Limitations: The reviewed product page did not evidence AI-specific opportunity discovery, responsible-AI governance, AI requirements/acceptance criteria, or AI pilot/adoption measurement. (Vendor page — absence of evidence in the reviewed source, not proof of absence.)

### EV-017 — Credo AI: AI governance platform (competitor)
- Organisation/author: Credo AI (vendor)
- Type: VENDOR (verified via product page)
- URL: https://www.credo.ai/
- Accessed: 2026-09-11
- Key finding (verified): AI use-case/system registry and shadow-AI discovery, continuous risk assessment, and policy mapping to regulations/frameworks (EU AI Act, NIST AI RMF, ISO 42001), with audit/evidence generation.
- Relevance: Strong on AI governance and use-case registration.
- Limitations: The reviewed product page did not evidence business-value discovery/prioritisation, requirements, ROI or adoption measurement. (Vendor page — absence of evidence in the reviewed source, not proof of absence.)

### EV-018 — IIBA: definition and scope of business analysis
- Organisation/author: International Institute of Business Analysis (IIBA)
- Type: PROF-BODY (official definition — authoritative)
- URL: https://www.iiba.org/professional-development/career-centre/what-is-business-analysis/
- Accessed: 2026-09-11
- Key finding (verified): IIBA's official definition — business analysis is "the practice of enabling change in an organizational context, by defining needs and recommending solutions that deliver value to stakeholders." Named activities include identifying/articulating change needs, defining value-maximising solutions, understanding required capabilities, and supporting change and continuous improvement.
- Relevance: Authoritative basis for the BA scope (defining needs; recommending value-delivering solutions) that underpins the workflow's BA-owned front half.
- Limitations: A definitional statement; the detailed task decomposition used in this project is BABOK-aligned BA practice (project interpretation), not established by this page alone.
