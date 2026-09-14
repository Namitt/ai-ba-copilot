# Validation Prototype, Software-MVP Boundary and Product-Necessity Challenge

Status: APPROVED
Owner: Namit Singh
Phase: 3 — Product Requirements
Basis: all Phase 3 requirement artefacts; PHASE2_SYNTHESIS conclusion; ASM-002/004/005/006/010.

> APPROVED — owner-approved as part of the Phase 3 Product Requirements baseline on 2026-09-14, after initial draft, owner CONDITIONAL PASS, amendments and final consistency review. Approval accepts this artefact as the current requirements baseline; it does NOT authorise a software build, Phase 4, or the pre-build validation gate (Phase 3.5). Prior review note: Distinguishes a PRE-BUILD VALIDATION PROTOTYPE from a CONDITIONAL SOFTWARE MVP, prioritises with MoSCoW, and performs the MANDATORY product-necessity challenge. It does not resolve the application-necessity question by assumption. The Phase 2 conclusion stands: an internally coherent operating model does NOT establish that a dedicated application is necessary. Nothing here authorises execution of the validation prototype or a build.

## 1. Two concepts

- **PRE-BUILD VALIDATION PROTOTYPE** — templates + Jira/Notion/Excel (or equivalent). Tests **ASM-002** and **ASM-004** before any build. **Not an application.** Recommended validation gate for owner decision; not authorised or started here. It does NOT require AI, and does NOT require detailed value-measurement planning.
- **CONDITIONAL SOFTWARE MVP** — only if the validation gate + owner decision justify custom software; scoped to capabilities where dedicated software materially improves control, enforcement, traceability or provenance.

## 2. MoSCoW prioritisation (capability level)

A capability is **MUST** only if (a) the core discipline hypothesis cannot be tested without it, (b) a hard governance/control requirement requires it, or (c) the approved process cannot operate coherently without it. AI-dependent controls are **CONDITIONAL MUST — IF AI ENABLED**. Measurement is SHOULD.

### MUST (discipline + non-negotiable controls; applies to the validation prototype)
- Capture request with problem/solution distinction (BR-001; FR-001/002).
- Evidence with explicit unknowns; no auto-fill (BR-002; FR-004/005/006; BRULE-005).
- Explicit AI-applicability consideration; where AI is credible, AI/non-AI/no-change compared with retained rejects; no fictional AI option (BR-003; FR-007/008; BRULE-010/012).
- Early governance capture + specialist disposition + hard-blocker gate (BR-004; FR-010/011/012/013; BRULE-002/007).
- Transparent prioritisation: gates separate from ranking; value cannot offset a gate (BR-007; FR-017/018; BRULE-003).
- Human control: AI never approves; where AI is used its output is marked unreviewed (BR-008; FR-026 conditional; BRULE-004).
- Decision with rationale/owners; park/stop retain rationale; traceability; authority separation across distinct dispositions (BR-006/009; FR-019/020/021/022/023/025/032; BRULE-006/008/009/011).
- Deterministic computation and auditability (NFR-001/006); authority-based access (NFR-003); proportionality (NFR-007).

### CONDITIONAL MUST — IF AI ENABLED
- AI-output provenance/marking, source-grounding, human edit/reject, safe degradation, AI transparency (FR-026/027/028/029; NFR-002). Mandatory whenever AI is included; **not** proof AI must be in the first prototype.

### SHOULD
- AI-assisted summary/options (FR-003/009 — also NEEDS VALIDATION).
- Value baseline & expected-vs-actual measurement (BR-005; FR-014/015/016) — conditional on ASM-006; NOT in the validation prototype.
- Provider independence & AI-assistance audit trail (FR-030/031; NFR-005).
- Reliability/recoverability, security-of-records (NFR-008/009).

### COULD
- Richer AI option generation (FR-009).

### CANDIDATE (retained, unproven source)
- Accessibility (NFR-010) — a genuine product-quality concern **if software is built**; no approved Phase 1/2 source, applicable standard to be set by an authorised phase. Not "polish", not selected here.

### OUT OF SCOPE (this phase)
- Pilot/adoption instrumentation, portfolio dashboards, integrations, automated evidence collection, multi-team scale (LATER); all UX/architecture/stack/AI-provider/code (Phases 4–6).

### NEEDS VALIDATION (must not be silently promoted to MUST)
- Whether a dedicated application is required at all (section 4); AI-assist necessity; adoption (ASM-004); measurement feasibility (ASM-006); market gap (RSK-001).

## 3. What the validation prototype is (and the "everything we want" guard)

The prototype is the smallest coherent slice to test: *does the BA-led discipline make AI opportunity decisions more consistent, defensible and traceable, and would users adopt it?* It deliberately **excludes** AI assistance, measurement instrumentation, portfolio views and integrations — including them would confound the test (is any improvement from the discipline, the AI, or dashboards?) and inflate effort (RSK-009).

## 4. PRODUCT-NECESSITY CHALLENGE (mandatory)

Taxonomy (revised per owner review — the key question is *custom product vs configurable existing tool*, not merely "software or not"):

- **P — PROCESS / TEMPLATE SUFFICIENT FOR VALIDATION**
- **C — CONFIGURABLE EXISTING TOOL MAY SUFFICE** (e.g. Jira workflow/permissions, Notion, a form tool)
- **X — CUSTOM PRODUCT MAY ADD MATERIAL VALUE**
- **V — NEEDS REAL-USER / HANDS-ON TOOL VALIDATION**

Assessed conservatively — hard-gate enforcement, role permissions and traceability are **not assumed** to require custom software; configurable tools may satisfy some or most.

| Capability | Class | Reasoning (conservative) |
|---|---|---|
| Problem/solution capture & framing | P / V | A structured template captures this; enforcement of the distinction could be a checklist. Needs user validation that it changes behaviour. |
| Evidence with explicit unknowns | P / V | Template with an "unknown" convention works; software value (preventing silent auto-fill) matters mainly once AI is involved. |
| AI-applicability + options (incl. non-AI) | P | A decision log / comparison table is adequate; the discipline is the point. |
| Early governance capture | P / C | Template or a configured form; a configurable tool can hold the fields. |
| Hard-gate enforcement (blocker stops progression; value can't override) | C / X / V | A configurable workflow tool (e.g. Jira statuses/permissions) can enforce *some* state transitions and block progression; whether that is sufficient vs a custom product that guarantees the no-override rule end-to-end needs hands-on tool validation. Not automatically custom. |
| Transparent prioritisation (gates vs ranking) | P / C | Documented method + spreadsheet, or a configured tool; a magic-score product is explicitly not the aim. |
| AI-output provenance/marking | X (only if AI used) | Reliable provenance/marking of AI output is awkward by hand — but only relevant if AI is in scope; a configurable tool may still suffice (V). |
| End-to-end traceability | C / X / V | Jira+Notion links give partial traceability; a configurable tool may extend it; whether a custom product's single navigable chain adds material value needs validation. |
| Authority-based access & multiple distinct dispositions | C | Configurable role/permission models in existing tools approximate this. |
| Controlled reopen-on-change | C / X | Rules can be documented and partly enforced in a configurable tool; custom enforcement is a maybe, not a given. |

### 4.1 "If AI BA Copilot did not exist as a dedicated application…"
Most of the approved operating model could be tested **by a first pre-build validation prototype** with structured templates + a configurable existing tool (Jira/Notion) for state, permissions and traceability, plus a spreadsheet for prioritisation arithmetic. Configurable tools can already enforce *some* state transitions, permissions and blocking. What a custom product **might** add is a guaranteed, integrated combination that is hard to assemble reliably from configured tools.

### 4.2 Remaining product value proposition (strongest current hypothesis)
The potential custom-product value lies in an **integrated combination** of: enforced control discipline · authority separation · provenance · traceability · controlled reopen/change behaviour — as one coherent operating control layer. This is a hypothesis about *integration value*, and **dedicated-product necessity remains UNPROVEN**. It is not established that any single control requires a custom build rather than a configured tool.

### 4.3 Honest conclusion
On current evidence, no capability is proven to *require* a dedicated custom product: templates and configurable existing tools plausibly cover the validation prototype, and possibly more. The strongest — still unproven — case for a custom product is the **integrated enforced-control-plus-traceability layer**, and even that must be tested against configurable tools hands-on (RSK-001; ASM-005) and against real users (ASM-002/004). **Phase 3 does not conclude that a dedicated application is necessary.**

## 5. Evidence still needed before build investment

- Real-user validation that the discipline changes decision quality/consistency (ASM-002) and that users adopt it without disproportionate burden (ASM-004).
- Hands-on evaluation of comparable tools AND of configuring an existing tool (Jira/Notion) to the discipline, to test whether custom software adds material value (RSK-001; ASM-005).
- Confirmation that value baselines are obtainable (ASM-006) before committing to measurement features.
- Evidence on whether inconsistent intake materially drives the value gap (ASM-010) — broader, not from a small pilot.

## Open questions

- OQ-M1: Authorise a **no-code validation prototype** (templates + Jira/Notion) to test ASM-002/004 before any build? (owner decision; not executed here)
- OQ-M2: If software is later built, scope it to the integrated enforced-control layer only?
- OQ-M3: Should a configurable-tool configuration be evaluated head-to-head against a custom build before any build decision?
