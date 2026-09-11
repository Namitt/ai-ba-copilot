# Phase 1 Discovery — Findings

Status: DRAFT
Owner: Namit Singh
Last Updated: 2026-09-11
Phase: 1 — Formal Discovery & Business Case

## Purpose

Consolidated Phase 1 findings across the five research streams. Each finding separates FACT / SOURCE CLAIM, INTERPRETATION, PROJECT IMPLICATION and ASSUMPTION, and references the source register ([EV-###] in research/sources/PHASE1_SOURCES.md). This is DRAFT evidence, not owner-approved conclusion.

---

## Stream A — Problem / demand & prioritisation

**F-A1**
- FACT / SOURCE CLAIM: Gartner predicts ≥30% of GenAI projects abandoned after PoC by end of 2025, citing unclear business value, poor data quality, cost and weak risk controls [EV-001]. MIT NANDA reports ~95% of enterprise GenAI pilots fail to deliver measurable P&L impact [EV-002].
- INTERPRETATION: A large share of AI demand is progressed without adequate problem framing, evidence, value definition or governance.
- PROJECT IMPLICATION: There is a genuine enterprise problem in how AI opportunities are qualified before investment — the space AI BA Copilot targets.
- ASSUMPTION: That better front-end BA discipline would materially change these outcomes (to be validated; see challenge in Stream E).

**F-A2**
- FACT / SOURCE CLAIM: Value-vs-feasibility scoring and portfolio framing of AI use cases are widely documented and commoditised [EV-009][EV-010].
- INTERPRETATION: Prioritisation mechanics are not novel; many tools and frameworks already do impact/effort scoring.
- PROJECT IMPLICATION: Differentiation cannot rest on "we prioritise use cases." It must rest on the evidenced, traceable, governed, measured operating discipline around prioritisation.
- ASSUMPTION: Buyers value discipline/traceability over a scoring widget (to be validated).

**F-A3 (what typically goes wrong)**
- FACT / SOURCE CLAIM: Reported failure causes cluster around unclear value, data/integration gaps, weak governance and poor adoption [EV-001][EV-002][EV-003].
- INTERPRETATION: Failure is mostly organisational and evidentiary, not model capability.
- PROJECT IMPLICATION: The workflow should force explicit evidence, value hypotheses, governance and measurement — not just idea capture.

## Stream B — BA in AI / innovation

**F-B1**
- FACT / SOURCE CLAIM: IIBA states AI assists synthesis and administrative work while BA judgement (technique selection, validation, accountability) stays human — "assistant, not authority" [EV-007].
- INTERPRETATION: The "AI assists, BA decides" control model is consistent with professional-body positioning.
- PROJECT IMPLICATION: Supports the product's core control model and human-approval gates.
- ASSUMPTION: None material; well aligned with established BA doctrine (BABOK-style discovery, elicitation, traceability).

**F-B2 (what belongs to a BA, not an engineer)**
- INTERPRETATION (from EV-007 plus standard BA practice): Problem framing, stakeholder analysis, current-state analysis, evidence gathering, options appraisal, requirements and acceptance criteria, benefits definition, and traceability are BA work; model building, data pipelines and deployment are engineering.
- PROJECT IMPLICATION: The workflow's front half is legitimately BA-owned; this is defensible, not inflated.
- ASSUMPTION: Kept honest — the product must not claim BA ownership of engineering feasibility, only of framing/evidence/value/governance capture.

## Stream C — Value / ROI / adoption

**F-C1**
- FACT / SOURCE CLAIM: McKinsey reports high adoption (65% gen AI in ≥1 function; ~72% overall) but early value capture — as reported, only 46 of 876 respondents attribute >10% of EBIT to gen AI [EV-003]. MIT reports most pilots show no P&L impact [EV-002].
- INTERPRETATION: There is a clear gap between deploying AI and realising business value.
- PROJECT IMPLICATION: The workflow must explicitly model: AI deployed ≠ AI adopted ≠ business value achieved, with baselines and expected-vs-actual measurement.
- ASSUMPTION: Organisations can capture baseline data; often they cannot (see risk).

**F-C2**
- FACT / SOURCE CLAIM: No defensible generic ROI percentage exists to reuse; figures are context-specific and reported value is early [EV-001][EV-003].
- INTERPRETATION: Any ROI in the business case must be stated as method + required baseline, not a fabricated number.
- PROJECT IMPLICATION: BUSINESS_CASE.md states benefit categories and measurement method, and explicitly flags that baseline data is required before numbers are credible.

## Stream D — Governance (UK-oriented)

**F-D1**
- FACT / SOURCE CLAIM: ICO applies UK GDPR principles to AI and expects DPIAs for high-risk processing (innovative tech, large-scale, automated decisions with significant effects, vulnerable individuals) [EV-004][EV-005]. DSIT sets five AI principles: safety/security/robustness, transparency/explainability, fairness, accountability/governance, contestability/redress [EV-006].
- INTERPRETATION: There is a concrete, recognised set of governance fields a UK AI workflow should capture.
- PROJECT IMPLICATION: The workflow should capture, per opportunity: personal-data use and DPIA trigger check, decision-significance/automation level, human-oversight point, fairness/bias consideration, transparency/explainability need, and accountable owner — mapped to the five principles.
- ASSUMPTION: A portfolio/demonstration project can model these without giving legal advice (explicitly non-legal-advice).

## Stream E — Existing solutions

**F-E1**
- FACT / SOURCE CLAIM: Adjacent categories exist and are mature: innovation-management platforms (ITONICS, HYPE, Brightidea, Planview IdeaPlace — vendor-described) [EV-008]; AI-driven strategic/project portfolio management (Planisware, Planview); and analyst use-case prioritisation offerings (Gartner AI Use Case Insights / portfolio guidance) [EV-009].
- INTERPRETATION: Idea intake, scoring, portfolio and funding views are already well served.
- PROJECT IMPLICATION: Overlap is real; see COMPARABLE_SOLUTIONS.md. Differentiation must be the BA-led operating discipline (evidence → options → value → requirements → pilot → measured outcome) with traceability, governance capture and human-approval gates — not idea funnelling or PPM.
- ASSUMPTION: No existing product combines all of these as a BA operating workflow (based on category scan, not exhaustive product testing — a limitation).

**F-E2 (challenge to the hypothesis)**
- FACT / SOURCE CLAIM: MIT attributes success more to integration, adaptation and line-level adoption than to front-end selection [EV-002].
- INTERPRETATION: Better discovery alone will not fix the value gap if adoption/integration is ignored.
- PROJECT IMPLICATION: The workflow must extend through pilot, adoption and outcome measurement — a discovery-only tool would not address the strongest evidenced failure cause.
- ASSUMPTION: The BA-led framing adds value beyond existing tools specifically because it carries evidence and measurement end-to-end (to be validated with stakeholder scenarios).
