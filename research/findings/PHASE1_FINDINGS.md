# Phase 1 Discovery — Findings

Status: DRAFT
Owner: Namit Singh
Last Updated: 2026-09-11
Phase: 1 — Formal Discovery & Business Case (owner-review amended)

## Purpose

Consolidated Phase 1 findings. Each finding separates **EVIDENCE** (what sources state) from **OUR HYPOTHESIS** (what we infer or propose, which is not yet demonstrated), with source references ([EV-###] in research/sources/PHASE1_SOURCES.md). DRAFT — not owner-approved conclusion.

> Correction note (owner review): earlier wording implied poor front-end BA discovery is a dominant *cause* of AI failure. The evidence does not establish that. Causal claims have been removed; the role of BA discipline is stated as a hypothesis to validate.

---

## Stream A — Problem / demand & prioritisation

**F-A1 — There is a large gap between AI activity and measured value.**
- EVIDENCE: Gartner *forecasts* ≥30% of GenAI projects abandoned after PoC by end-2025 (a prediction, not an observed rate) [EV-001]. MIT NANDA (preliminary) reports ~95% of organisations see no measurable P&L return, with ~5% of integrated pilots capturing significant value [EV-002]. McKinsey 2026 reports 37% attribute positive EBIT contribution and 44% scaling enterprise-wide despite ~90% regular use [EV-011].
- OUR HYPOTHESIS: Better-qualified demand and disciplined discovery *could* reduce wasted effort. This is not demonstrated by the evidence.

**F-A2 — Prioritisation is widely available across the reviewed offerings/frameworks.**
- EVIDENCE: Value-vs-feasibility scoring and portfolio framing are widely documented across analyst, vendor and practitioner sources [EV-009][EV-010][EV-015][EV-016].
- OUR HYPOTHESIS: Differentiation cannot rest on prioritisation; if there is value, it lies in evidenced, traceable, governed, measured operating discipline. To validate.

**F-A3 — Reported problems are multiple, not a single BA-discovery cause.**
- EVIDENCE: Reported contributors span unclear value, data/integration challenges, governance immaturity, adoption, measurement and operating-model/workflow issues [EV-001][EV-002][EV-011][EV-012].
- OUR HYPOTHESIS: A structured BA-led process *might* improve consistency across framing, evidence, options, governance and measurement. Explicitly a hypothesis.

## Stream B — BA in AI / innovation

**F-B1 — AI assists; the BA decides.**
- EVIDENCE: IIBA states AI accelerates synthesis/admin while BA judgement and accountability remain human — "assistant, not authority" [EV-007].
- OUR HYPOTHESIS: None needed — this supports the control model directly.

**F-B2 — What plausibly belongs to a BA.**
- EVIDENCE: IIBA's official definition frames business analysis as "enabling change ... by defining needs and recommending solutions that deliver value to stakeholders" [EV-018]; IIBA also describes AI as assistant to BA judgement [EV-007].
- PROJECT INTERPRETATION / SCOPE: Building on that definition, standard BABOK-aligned BA practice includes problem framing, stakeholder analysis, current-state analysis, evidence gathering, options appraisal, requirements/acceptance criteria, benefits definition and traceability; model building, data pipelines and deployment are engineering. This task decomposition reflects common BA practice to be validated in the project — not a claim evidenced by EV-007 alone.
- We do not claim BA ownership of engineering feasibility.

## Stream C — Value / ROI / adoption

**F-C1 — Adoption is high; enterprise value lags.**
- EVIDENCE: McKinsey 2026 — ~90% regular use, 44% scaling, 37% positive EBIT contribution, ~1 in 5 constrained by operating costs [EV-011]. McKinsey Apr 2026 — ~80% deploy gen AI yet ~60% report no enterprise-wide EBIT impact [EV-012]. (2024 baseline retained for comparison [EV-003].)
- OUR HYPOTHESIS: Modelling deployed ≠ adopted ≠ value, with baselines and expected-vs-actual measurement, *could* help close the gap. To validate.

**F-C2 — A concrete measurement method exists.**
- EVIDENCE: McKinsey proposes a five-layer measurement framework (technical → adoption → operational → strategic → financial) and building measurement into rollout with governance gates and evidence packs [EV-012].
- PROJECT IMPLICATION: The business case states a measurement method rather than a fabricated ROI; the five-layer model is a candidate structure. Baseline data is required before any ROI figure.

## Stream D — Governance (UK-oriented; Sept 2026)

**F-D1 — Law/regulatory guidance vs government practice guidance are distinct.**
- EVIDENCE (LAW/REG): ICO applies UK GDPR to AI [EV-004]; DPIAs required for high-risk processing [EV-005]; the DUAA 2025 (data-protection provisions in force by 19 Jun 2026) expands lawful bases for significant automated decisions with safeguards, excluding special category data [EV-013].
- EVIDENCE (GOV-POLICY): DSIT's five AI principles [EV-006] — explicitly non-statutory.
- EVIDENCE (GOV-PRACTICE): the UK Government AI Playbook [EV-014] (Feb 2025, GDS) — explicitly practice guidance for government, not law for private organisations; ten practical principles incl. meaningful human control, full AI lifecycle, right tool for the job, assurance and early commercial involvement.
- PROJECT IMPLICATION: Per opportunity, capture: personal-data use + DPIA trigger check; ADM significance/automation level and its DUAA-era safeguard/lawful basis; human-oversight point; fairness/transparency need; accountable owner. Keep LAW/REG separate from PRACTICE; this is not legal advice.

## Stream E — Existing solutions

**F-E1 — Adjacent solution categories cover substantial parts of the workflow.**
- EVIDENCE: IT/application AI-transformation assessment (IBM Txture — 5A method, ROI quantification) [EV-015]; strategic portfolio management (Planview — intake→prioritise→fund→track→benefits) [EV-016]; AI governance (Credo AI — use-case registry, risk, policy mapping) [EV-017]; innovation management (ITONICS, vendor) [EV-008]; analyst prioritisation (Gartner) [EV-009]. See COMPARABLE_SOLUTIONS.md.
- OUR HYPOTHESIS: No single evidenced product combines BA-led discovery + options + responsible-AI capture + requirements + pilot/adoption/value measurement + traceability as one operating workflow. Stated as a **potential gap** hypothesis, not proven whitespace.

**F-E2 — Value realisation depends on more than discovery.**
- EVIDENCE: MIT emphasises integration, adaptation and adoption as important contributors to value realisation [EV-002]; McKinsey emphasises measurement and operating-model factors [EV-012]. These sources do not establish that front-end discovery is unimportant.
- PROJECT IMPLICATION (hypothesis): Discovery alone is unlikely to be sufficient; the proposed workflow therefore tests an end-to-end model through adoption and outcome measurement.
