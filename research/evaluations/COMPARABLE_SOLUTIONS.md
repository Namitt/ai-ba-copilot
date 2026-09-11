# Phase 1 Discovery — Comparable Solutions Evaluation

Status: APPROVED
Owner: Namit Singh
Last Updated: 2026-09-11
Phase: 1 — Formal Discovery & Business Case (owner-approved baseline)

> Owner-approved as the Phase 1 discovery baseline on 2026-09-11 (baseline commit fb5f23f). Approval accepts this documentation-based evaluation as the current baseline; the potential-gap conclusion remains a hypothesis (market whitespace not proven).

## Purpose

Second-pass evaluation of representative solutions that overlap with AI BA Copilot, using direct product/primary documentation wherever practical, to test whether a potential gap exists. The objective is not to say competitors are weak; it is to locate any gap honestly.

## Evidence status key

Each attribute is marked **VERIFIED** (stated on the product/primary page accessed 2026-09-11), **PARTIALLY VERIFIED** (from a vendor blog or analyst abstract, not a full product page), or **NOT EVIDENCED** (not confirmed from an accessible source — an absence of evidence, not proof of absence). Low/Medium/High judgements are avoided.

## Solutions evaluated (5)

### 1. IBM Txture — AI transformation planning & assessment [EV-015]
- Source: IBM product page — VERIFIED.
- Target user: enterprise IT leadership, application-portfolio managers.
- Verified capabilities: IT/application landscape assessment from CMDB/EA data; AI use-case identification via "5A" method; segmentation into quick wins/strategic bets/delivery waves; effort, cost, payback and multi-year benefit quantification.
- Opportunity intake: application-portfolio-driven — VERIFIED. Business pain-point intake: NOT EVIDENCED.
- Discovery/problem framing: NOT EVIDENCED (starts from application inventory).
- Prioritisation: VERIFIED (5A scoring, waves).
- Value/ROI: VERIFIED (payback, first-year, three-year benefit).
- Governance (responsible-AI): NOT EVIDENCED.
- Requirements/delivery: NOT EVIDENCED.
- Pilot/measurement, adoption measurement, traceability: NOT EVIDENCED.
- Overlap: prioritisation and ROI quantification. Potential gap / capability not evidenced in reviewed source: business discovery, governance capture, requirements, adoption/outcome measurement.

### 2. Planview — Strategic Portfolio Management [EV-016]
- Source: Planview product page — VERIFIED.
- Target user: CFO/board, transformation office, EPMO/PMO, finance.
- Verified capabilities: demand intake (unstructured ideas → formal requests); investment prioritisation (what-if, business drivers); funding/roadmaps; delivery tracking; investment-to-outcome and benefits/ROI tracking.
- Opportunity intake: VERIFIED (general demand, not AI-specific).
- Discovery/problem framing: NOT EVIDENCED (portfolio/PPM, not BA discovery).
- Prioritisation: VERIFIED. Value/ROI: VERIFIED (benefits realisation).
- Governance (responsible-AI): NOT EVIDENCED (enterprise controls, not AI-specific).
- Requirements/delivery: PARTIALLY VERIFIED (delivery tracking; not AI requirements/acceptance criteria).
- Pilot/adoption measurement for AI: NOT EVIDENCED. Traceability: PARTIALLY VERIFIED (investment-to-outcome).
- Overlap: intake→prioritise→fund→track→benefits. Potential gap / capability not evidenced in reviewed source: AI-specific discovery, responsible-AI capture, AI requirements and adoption measurement.

### 3. Credo AI — AI governance platform [EV-017]
- Source: Credo AI product page — VERIFIED.
- Target user: enterprises scaling AI under governance (financial services, health, public sector).
- Verified capabilities: AI use-case/system registry and shadow-AI discovery; continuous risk assessment; policy mapping to EU AI Act/NIST AI RMF/ISO 42001; audit/evidence.
- Opportunity intake: PARTIALLY VERIFIED (registration of AI systems/use cases, governance-oriented, not business-value intake).
- Discovery/problem framing: NOT EVIDENCED. Prioritisation by value: NOT EVIDENCED.
- Value/ROI: NOT EVIDENCED. Governance: VERIFIED (its core).
- Requirements/delivery: NOT EVIDENCED. Pilot/adoption/value measurement: NOT EVIDENCED. Traceability: VERIFIED (governance evidence/audit).
- Overlap: governance capture and traceability. Potential gap / capability not evidenced in reviewed source: business discovery, value definition, prioritisation, requirements, outcome measurement.

### 4. ITONICS — innovation management [EV-008]
- Source: vendor blog — PARTIALLY VERIFIED.
- Target user: innovation/transformation teams.
- Capabilities (vendor claim): foresight, ideation, portfolio; idea intake → scoring → portfolio/roadmap.
- Opportunity intake: PARTIALLY VERIFIED. Discovery/problem framing: NOT EVIDENCED. Prioritisation: PARTIALLY VERIFIED.
- Value/ROI, governance, requirements, pilot/adoption measurement, traceability: NOT EVIDENCED.
- Overlap: idea intake and prioritisation. Potential gap / capability not evidenced in reviewed source: evidence-led BA discovery, governance, requirements, measurement.

### 5. Gartner AI Use Case Insights / portfolio guidance [EV-009]
- Source: analyst product page/abstract — PARTIALLY VERIFIED (paywalled).
- Target user: leaders selecting/funding AI investments.
- Capabilities: catalogue, benchmarked value/feasibility prioritisation, funding guidance.
- Opportunity intake: PARTIALLY VERIFIED. Discovery/problem framing: NOT EVIDENCED. Prioritisation: PARTIALLY VERIFIED. Value/ROI: PARTIALLY VERIFIED.
- Governance, requirements, pilot/adoption measurement, traceability: NOT EVIDENCED (advisory content, not an operating workflow).
- Overlap: prioritisation guidance. Potential gap / capability not evidenced in reviewed source: an operating workflow carrying one pain point end-to-end with traceability.

## Overlap summary (evidence-qualified)

| Capability | Txture | Planview | Credo AI | ITONICS | Gartner |
|---|---|---|---|---|---|
| Business pain-point intake | Not evidenced | Verified (general) | Partial (gov) | Partial | Partial |
| Evidence-led BA discovery | Not evidenced | Not evidenced | Not evidenced | Not evidenced | Not evidenced |
| Prioritisation | Verified | Verified | Not evidenced | Partial | Partial |
| Responsible-AI governance capture | Not evidenced | Not evidenced | Verified | Not evidenced | Not evidenced |
| Requirements + acceptance criteria | Not evidenced | Partial | Not evidenced | Not evidenced | Not evidenced |
| Value model (deployed≠adopted≠value) | Partial (ROI) | Partial (benefits) | Not evidenced | Not evidenced | Partial |
| Pilot + adoption/outcome measurement | Not evidenced | Not evidenced | Not evidenced | Not evidenced | Not evidenced |
| End-to-end traceability | Not evidenced | Partial | Verified (gov) | Not evidenced | Not evidenced |

## Conclusion

The reviewed products provide substantial capabilities in prioritisation, portfolio management and AI governance. Across the five evaluated, no single product was evidenced to combine BA-led discovery, responsible-AI capture, requirements, and pilot/adoption/outcome measurement as one traceable operating workflow.

**Our current hypothesis is that a potential gap exists** for such a BA-led operating workflow. This is a hypothesis, not proven market whitespace: the scan is documentation-based (not hands-on), several attributes are only PARTIALLY VERIFIED or NOT EVIDENCED, and evidence [EV-002][EV-012] indicates adoption/integration and measurement — not discovery — are the harder problems, so any gap must be tested by hands-on evaluation and stakeholder scenarios before it is claimed.
