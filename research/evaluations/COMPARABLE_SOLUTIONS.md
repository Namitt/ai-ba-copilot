# Phase 1 Discovery — Comparable Solutions Evaluation

Status: DRAFT
Owner: Namit Singh
Last Updated: 2026-09-11
Phase: 1 — Formal Discovery & Business Case

## Purpose

Assess existing product/framework categories that overlap with AI BA Copilot, to test whether there is genuine space for a BA-led operating workflow. The objective is not to say competitors are weak; it is to locate the gap honestly. Vendor descriptions are labelled as vendor claims and were not independently tested.

## Method and limitation

Category-level scan from analyst, vendor and practitioner sources ([EV-008][EV-009][EV-010]); no hands-on product trials were performed. Conclusions are DRAFT and should be validated by hands-on evaluation of one or two representative tools.

## Categories assessed

### 1. Innovation / idea management platforms
- Examples (vendor-described [EV-008]): ITONICS, HYPE, Brightidea, Planview IdeaPlace, Qmarkets.
- Target user: innovation teams, transformation offices.
- Core workflow: signal/trend → idea intake → scoring/voting → portfolio/roadmap.
- Prioritisation: scoring, ML theming, gamified voting.
- Value/ROI: portfolio dashboards; limited rigorous baseline/benefit measurement.
- Governance: generally not AI-governance specific.
- Requirements/delivery: not a BA requirements tool.
- Measurement/adoption: participation and pipeline metrics rather than outcome realisation.
- Strengths: strong at capturing and funnelling many ideas.
- Gaps vs our concept: not evidence-led BA discovery; weak on options appraisal, requirements, AI-specific governance and expected-vs-actual outcome measurement.

### 2. Strategic / project portfolio management (SPM/PPM)
- Examples: Planisware, Planview (AI-driven SPM capabilities).
- Target user: PMO, portfolio leaders, finance.
- Core workflow: demand → prioritisation → funding → delivery tracking.
- Prioritisation: value/cost/capacity, scenario planning.
- Value/ROI: financial planning strong; AI-value nuance (deployed vs adopted vs value) not specific.
- Governance: enterprise controls, not AI-responsible-AI capture.
- Strengths: funding, capacity, executive portfolio view.
- Gaps vs our concept: heavyweight, delivery/finance-oriented; not a BA discovery + AI-opportunity + responsible-AI workflow.

### 3. Analyst use-case prioritisation offerings
- Examples: Gartner AI Use Case Insights / "vet, prioritize and fund AI use cases" [EV-009].
- Target user: leaders selecting/funding AI investments.
- Core workflow: catalogue → score → portfolio funding guidance.
- Prioritisation: analyst-grade value/feasibility.
- Strengths: credible, benchmarked prioritisation.
- Gaps vs our concept: advisory/benchmarking content and scoring, not an operating workflow that carries a single pain point through evidence, requirements, pilot and measured outcome with traceability.

### 4. Data-science / AI platforms
- Examples (category): Dataiku, DataRobot, cloud AI suites (not separately fetched).
- Target user: data science / ML engineering.
- Core workflow: build → deploy → monitor models.
- Gaps vs our concept: engineering-centric; assume the opportunity is already chosen and framed — the BA front-half is out of scope for them.

## Overlap summary

| Capability | Innovation mgmt | SPM/PPM | Analyst prioritiser | DS platforms | AI BA Copilot (proposed) |
|---|---|---|---|---|---|
| Idea/pain-point intake | Strong | Medium | Low | Low | Core |
| Evidence-led BA discovery | Low | Low | Low | Low | Core (differentiator) |
| Prioritisation | Strong | Strong | Strong | Low | Included (not the differentiator) |
| AI vs non-AI options appraisal | Low | Low | Medium | Low | Core |
| Requirements + acceptance criteria | Low | Low | Low | Low | Core |
| Responsible-AI / governance capture | Low | Medium | Medium | Medium | Core (differentiator) |
| Value model: deployed≠adopted≠value | Low | Medium | Medium | Low | Core (differentiator) |
| Pilot + expected-vs-actual measurement | Low | Medium | Low | Medium | Core (differentiator) |
| Traceability + human-approval gates | Low | Medium | Low | Low | Core (differentiator) |

## Conclusion (DRAFT)

Prioritisation and idea/portfolio management are well served and should not be claimed as novel. The unoccupied space is a **BA-led operating workflow with end-to-end traceability** that takes a single business pain point from evidence and options appraisal through responsible-AI governance capture, requirements, pilot and expected-vs-actual outcome measurement, with explicit human-approval gates. This differentiation is **plausible but partial**, and is challenged by evidence [EV-002] that adoption/integration — not discovery — is the dominant failure cause; the product must therefore prove value across the whole journey, not just the front end.
