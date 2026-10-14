![Global Operations](assets/banners/global-operation.jpg)

# AI Business Development Toolkit

### Commercial Intelligence | International Business Development | GTM | Strategic Partnerships

![Discovery](https://img.shields.io/badge/IDENTIFY-v1.0.0-success)
![Lead Qualification](https://img.shields.io/badge/PRIORITIZE-v2.0.0-success)
![Adaptive Outreach](https://img.shields.io/badge/ENGAGE-v2.1.0-success)
![Partnership Intelligence](https://img.shields.io/badge/PARTNER-v2.0.0-success)
![Market Expansion](https://img.shields.io/badge/ROADMAP-Market%20Expansion-orange)
![License](https://img.shields.io/badge/License-All%20Rights%20Reserved-lightgrey)

A connected portfolio of Commercial Intelligence applications built to make Business Development decisions more **structured, explainable and actionable**.

The portfolio combines deterministic commercial logic, public evidence, portable handoffs and optional AI assistance.

> **The objective is not technology for technology's sake. The objective is better commercial judgment and execution.**

---

## Portfolio Architecture

The toolkit uses two coordinated commercial tracks.

```text
COMMERCIAL MANDATE
Client · Corridor · Product · Objective · Buyers / Partners · Route to Market
        ↓

ACCOUNT DEVELOPMENT

IDENTIFY
Market Entry & Opportunity Intelligence
        ↓
PRIORITIZE
Counterparty Qualification & Commercial Priority
        ↓
ENGAGE
Business Development Execution
        ↓
Qualified Dialogue → Opportunity → Deal Sheet → Mandate Reporting


PARTNERSHIP DEVELOPMENT

IDENTIFY / Partner Universe
        ↓
PARTNER
Route-to-Market & Partner Intelligence
        ↓
ENGAGE
Partner Development & Follow-Up
        ↓
Qualified Dialogue → Opportunity → Mandate Reporting


ROADMAP
Standalone Market Expansion Intelligence
```

Each layer has a specific commercial purpose. The system does not force every opportunity through one universal funnel.

---

## Commercial Mandate Layer

The portfolio now shares a portable **Commercial Mandate** across the shipped applications.

The mandate can preserve:

- represented company / client
- origin → target commercial corridor
- product / solution
- commercial objective
- buyer vs partner focus
- target buyer and partner types
- route-to-market hypothesis
- value proposition
- HS / CN / NCM references where available
- target territories and working languages
- success criteria

For cross-border work, the workflow can also preserve **Trade & Market Entry Feasibility** verification states covering tariff scenarios, preferential treatment, Ex-Tarifário relevance, rules of origin, import requirements, technical requirements and after-sales needs.

These states organize commercial execution; they are not automatic customs, legal, tariff or technical conclusions.

**Contracts:**
- [Commercial Mandate Contract v1](contracts/commercial-mandate-contract-v1.md)
- [Trade & Market Entry Feasibility Contract v1](contracts/trade-feasibility-contract-v1.md)
- [Commercial Intelligence Data Contract v1](contracts/commercial-intelligence-data-contract-v1.md)

### Ambrosin Commercial Mandate Workspace

The live applications now expose the same **Mandate Workspace** navigation layer.

From any module, the user can see:

- the active Commercial Mandate when one is loaded
- the current workflow stage
- the recommended next stage
- direct navigation to IDENTIFY, PRIORITIZE, PARTNER and ENGAGE
- the same portable Commercial Mandate JSON as the cross-app context carrier

This turns the portfolio into a modular Business Development operating workflow rather than four isolated applications.

Detailed reference: [Ambrosin Commercial Mandate Workspace](docs/MANDATE_WORKSPACE.md)

---

## Current Applications

| Layer | Application | Version | Commercial Purpose | Live |
|---|---|---:|---|---|
| **IDENTIFY** | [Opportunity Discovery Intelligence](https://github.com/Eambrosin/opportunity-discovery-intelligence) | v1.0.0 | Frame a Commercial Mandate, assess trade-feasibility questions, and discover buyer / partner universes using public evidence | [Launch](https://opportunity-discovery-intelligence-eambrosin.streamlit.app/) |
| **PRIORITIZE** | [Lead Qualification & Revenue Prioritization](https://github.com/Eambrosin/lead-qualification-scorer) | v2.0.0 | Qualify counterparties in the context of the mandate and allocate commercial attention using explainable scoring | [Launch](https://lead-qualification-scorer-eambrosin.streamlit.app/) |
| **ENGAGE** | [Adaptive Outreach Intelligence](https://github.com/Eambrosin/outreach-sequence-generator) | v2.1.0 | Execute outreach, qualification dialogue, follow-up, opportunity tracking, deal sheets and mandate reporting | [Launch](https://outreach-sequence-generator-eambrosin.streamlit.app/) |
| **PARTNER** | [Partnership Intelligence](https://github.com/Eambrosin/partnership-opportunity-finder) | v2.0.0 | Evaluate route-to-market fit, market access, technical / after-sales capability and execution feasibility | [Launch](https://partnership-opportunity-finder-eambrosin.streamlit.app/) |

---

## IDENTIFY — Market Entry & Opportunity Intelligence

**Commercial question:** For this mandate, who could buy or enable market entry, what public evidence supports the hypothesis, and what must still be validated?

Core capabilities include:

- configurable, sector-adaptive target-market profiles
- photovoltaic C&I end-customer discovery
- Medicina Estetica opportunity discovery
- public-web discovery
- explainable candidate ranking
- Account Opportunity
- Qualification Readiness
- account enrichment
- public-contact validation
- public LinkedIn profile discovery
- territory intelligence
- sector-specific operational / technology evidence
- Sales Intelligence
- qualification questions and evidence gaps
- direct handoffs to PRIORITIZE and ENGAGE

**Repository:** [opportunity-discovery-intelligence](https://github.com/Eambrosin/opportunity-discovery-intelligence)  
**Live App:** [Launch IDENTIFY](https://opportunity-discovery-intelligence-eambrosin.streamlit.app/)

---

## PRIORITIZE — Counterparty Qualification & Commercial Priority

**Commercial question:** Which counterparties matter most to this mandate, how complete is the qualification evidence, and what should happen next?

Core capabilities include:

- configurable Ideal Customer Profile
- weighted commercial scoring
- explainable score breakdown
- priority tiers
- revenue context
- executive account workspace
- recommended next actions
- research / readiness context
- optional AI-assisted account interpretation
- ENGAGE handoff

**Repository:** [lead-qualification-scorer](https://github.com/Eambrosin/lead-qualification-scorer)  
**Live App:** [Launch PRIORITIZE](https://lead-qualification-scorer-eambrosin.streamlit.app/)

---

## ENGAGE — Business Development Execution

**Commercial question:** How should we approach the counterparty, progress the dialogue, manage follow-up and advance a qualified opportunity toward commercial execution?

Core capabilities include:

- qualification-aware outreach strategy
- Buyer Access and Sales Motion context
- priority-based cadence
- public-channel-aware execution
- multilingual outreach
- qualification-first messaging
- Business Development execution log
- response / meeting / next-action tracking
- Commercial Deal Sheet
- mandate-level activity and pipeline reporting
- deterministic fallback generation
- optional AI-assisted copy
- territory / field-sales context
- visit-feedback loop
- upstream handoff compatibility

**Current Release:** **v2.1.0**

**Repository:** [outreach-sequence-generator](https://github.com/Eambrosin/outreach-sequence-generator)  
**Live App:** [Launch ENGAGE](https://outreach-sequence-generator-eambrosin.streamlit.app/)

---

## PARTNER — Route-to-Market & Partner Intelligence

**Commercial question:** Which partners can create credible market access and execution capability for this mandate, and what relationship model makes sense?

Core capabilities include:

- configurable partnership strategy
- explainable weighted scoring
- strategic-fit assessment
- market-access context
- relationship-strength signals
- execution feasibility
- route-to-market due diligence
- customer-base fit
- technical-service and after-sales capability
- import / regulatory capability
- exclusivity-conflict validation
- partnership archetypes
- recommended partnership models
- opportunity-level workspace
- recommended next action

**Repository:** [partnership-opportunity-finder](https://github.com/Eambrosin/partnership-opportunity-finder)  
**Live App:** [Launch PARTNER](https://partnership-opportunity-finder-eambrosin.streamlit.app/)

---

## Shared Commercial Intelligence Principles

### Evidence before interpretation

Observed information, research gaps and commercial hypotheses remain distinguishable.

### Explainable logic

Commercial scoring and prioritization should be traceable to configured criteria.

### Portable context

Upstream reasoning should move downstream instead of being rebuilt at every stage.

### AI as assistance

AI can support research, interpretation and communication. It does not silently determine the underlying commercial score or convert missing information into certainty.

### Human judgment

The tools support Business Development decisions; they do not replace qualification conversations, due diligence, negotiation or management approval.

---

## Shared Data Contracts

The applications use portable handoffs and common metadata to preserve commercial context across stages.

Current shared contracts:

- [Commercial Intelligence Data Contract v1](contracts/commercial-intelligence-data-contract-v1.md)
- [Commercial Mandate Contract v1](contracts/commercial-mandate-contract-v1.md)
- [Trade & Market Entry Feasibility Contract v1](contracts/trade-feasibility-contract-v1.md)
- [Market Profile Registry v1](contracts/market-profile-registry-v1.md)

Shared concepts include:

- `schema_version`
- `source_stage`
- `market_profile_id`
- Commercial Mandate
- buyer / partner counterparty focus
- trade-feasibility verification states
- account identity
- score rationale
- Qualification Readiness
- Buyer Access
- Sales Motion
- qualification gaps
- recommended next action
- opportunity / deal context
- mandate reporting

---

## Commercial Frameworks Behind the Tools

Technology is only one layer of the portfolio.

The underlying Business Development methods are maintained in:

**[Business Development Frameworks & Playbooks](https://github.com/Eambrosin/bd-frameworks-and-playbooks)**

That repository includes:

- experience-based commercial cases
- market-entry frameworks
- strategic-partnership frameworks
- distributor-selection tools
- partner due-diligence tools
- 90-day market-entry planning

---

## Experience Behind the Portfolio

The tools are informed by practical commercial experience across:

- B2B and B2G Business Development
- public procurement
- multi-site contract execution
- renewable energy
- international photovoltaic sourcing
- international trade
- strategic partnerships
- cross-border market development

The portfolio is intended to demonstrate how commercial experience can be translated into repeatable decision systems.

---

## Technology

Current applications use technologies including:

- Python
- Streamlit
- Pandas
- Plotly
- public-web research APIs
- optional LLM APIs
- GitHub Actions
- automated tests

Technology is treated as an execution layer, not the professional identity of the portfolio.

---

## Roadmap — Market Expansion Intelligence

**Status:** Roadmap / not presented as a shipped product.

Market-expansion functionality is now partially operationalized across the shipped applications through Commercial Mandate, trade-feasibility, buyer / partner discovery, route-to-market due diligence, execution tracking, deal sheets and reporting.

A **separate standalone Market Expansion Intelligence application** remains a roadmap item and will not be presented as shipped until it reaches the same implementation, testing and demo standard as IDENTIFY, PRIORITIZE, ENGAGE and PARTNER.

For the concise roadmap:

[View ROADMAP.md](ROADMAP.md)

---

## Repository Map

```text
README.md
ROADMAP.md

contracts/
  commercial-intelligence-data-contract-v1.md
  commercial-mandate-contract-v1.md
  trade-feasibility-contract-v1.md
  market-profile-registry-v1.md

intelligence/
  market-expansion-analysis.md

assets/
  banners/
  screenshots/

docs/
  PORTFOLIO_ARCHITECTURE_REFERENCE.md
  ROADMAP_REFERENCE.md
```

---

## Limitations

This toolkit is a portfolio and commercial decision-support ecosystem.

It does not:

- autonomously make commercial commitments
- replace CRM governance
- verify private contact information
- infer purchase intent from an internal score
- replace market, legal, regulatory or financial due diligence
- replace human judgment before external action

---

## Detailed Reference

The previous long-form architecture documentation is preserved here:

[Detailed Portfolio Architecture Reference](docs/PORTFOLIO_ARCHITECTURE_REFERENCE.md)

---

## Professional Positioning

**Eduardo Ambrosin**  
International Business Development | Strategic Partnerships | GTM | Commercial Intelligence

[GitHub Profile](https://github.com/Eambrosin) · [LinkedIn](https://www.linkedin.com/in/eduardoambrosin/) · [Professional Website](https://www.ambrosinlegaltrade.com/)
