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
ACCOUNT DEVELOPMENT

IDENTIFY
Opportunity Discovery Intelligence
        ↓
PRIORITIZE
Lead Qualification & Revenue Prioritization
        ↓
ENGAGE
Adaptive Outreach Intelligence


PARTNERSHIP DEVELOPMENT

IDENTIFY / Partner Universe
        ↓
PARTNER
Partnership Intelligence
        ↓
ENGAGE
Adaptive Partner Outreach


ROADMAP
Market Expansion Intelligence
```

Each layer has a specific commercial purpose. The system does not force every opportunity through one universal funnel.

---

## Current Applications

| Layer | Application | Version | Commercial Purpose | Live |
|---|---|---:|---|---|
| **IDENTIFY** | [Opportunity Discovery Intelligence](https://github.com/Eambrosin/opportunity-discovery-intelligence) | v1.0.0 | Discover and screen target accounts using public evidence and market-specific criteria | [Launch](https://opportunity-discovery-intelligence-eambrosin.streamlit.app/) |
| **PRIORITIZE** | [Lead Qualification & Revenue Prioritization](https://github.com/Eambrosin/lead-qualification-scorer) | v2.0.0 | Allocate attention using configurable ICP and explainable commercial scoring | [Launch](https://lead-qualification-scorer-eambrosin.streamlit.app/) |
| **ENGAGE** | [Adaptive Outreach Intelligence](https://github.com/Eambrosin/outreach-sequence-generator) | v2.1.0 | Convert qualification context into channel-aware, multilingual outreach | [Launch](https://outreach-sequence-generator-eambrosin.streamlit.app/) |
| **PARTNER** | [Partnership Intelligence](https://github.com/Eambrosin/partnership-opportunity-finder) | v2.0.0 | Evaluate strategic fit, market access and execution feasibility | [Launch](https://partnership-opportunity-finder-eambrosin.streamlit.app/) |

---

## IDENTIFY — Opportunity Discovery Intelligence

**Commercial question:** Which accounts should enter the pipeline, and what evidence supports that decision?

Core capabilities include:

- configurable target-market profiles
- public-web discovery
- explainable candidate ranking
- Account Opportunity
- Qualification Readiness
- account enrichment
- public-contact validation
- public LinkedIn profile discovery
- territory intelligence
- Sales Intelligence
- qualification questions and evidence gaps
- direct handoffs to PRIORITIZE and ENGAGE

**Repository:** [opportunity-discovery-intelligence](https://github.com/Eambrosin/opportunity-discovery-intelligence)  
**Live App:** [Launch IDENTIFY](https://opportunity-discovery-intelligence-eambrosin.streamlit.app/)

---

## PRIORITIZE — Lead Qualification & Revenue Prioritization

**Commercial question:** Which opportunities deserve attention first, and why?

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

## ENGAGE — Adaptive Outreach Intelligence

**Commercial question:** How should this opportunity be approached, through which available channel and with what cadence?

Core capabilities include:

- qualification-aware outreach strategy
- Buyer Access and Sales Motion context
- priority-based cadence
- public-channel-aware execution
- multilingual outreach
- qualification-first messaging
- deterministic fallback generation
- optional AI-assisted copy
- territory / field-sales context
- visit-feedback loop
- upstream handoff compatibility

**Current Release:** **v2.1.0**

**Repository:** [outreach-sequence-generator](https://github.com/Eambrosin/outreach-sequence-generator)  
**Live App:** [Launch ENGAGE](https://outreach-sequence-generator-eambrosin.streamlit.app/)

---

## PARTNER — Partnership Intelligence

**Commercial question:** Which partnership opportunities should be prioritized, and what relationship model makes sense?

Core capabilities include:

- configurable partnership strategy
- explainable weighted scoring
- strategic-fit assessment
- market-access context
- relationship-strength signals
- execution feasibility
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
- [Market Profile Registry v1](contracts/market-profile-registry-v1.md)

Shared concepts include:

- `schema_version`
- `source_stage`
- `market_profile_id`
- account identity
- score rationale
- Qualification Readiness
- Buyer Access
- Sales Motion
- qualification gaps
- recommended next action

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

The future Market Expansion Intelligence layer is intended to structure market-entry decisions around commercial fit, route to market, partnership need, localization, execution complexity and validation questions.

It remains outside the shipped product set until it reaches the same implementation, testing and demo standard as IDENTIFY, PRIORITIZE, ENGAGE and PARTNER.

For the concise roadmap:

[View ROADMAP.md](ROADMAP.md)

---

## Repository Map

```text
README.md
ROADMAP.md

contracts/
  commercial-intelligence-data-contract-v1.md
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
