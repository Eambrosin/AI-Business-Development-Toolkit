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

The portfolio combines deterministic commercial logic, public evidence, a shared private Commercial Mandate Workspace, role-aware handoffs and optional AI assistance.

> **The objective is not technology for technology's sake. The objective is better commercial judgment and execution.**

---


## Portfolio Architecture

The toolkit is organized around one persistent **Commercial Mandate** and two coordinated commercial tracks.

```text
COMMERCIAL MANDATE
Client · Corridor · Product · Objective · Buyers / Partners · Route to Market
        ↓
Private Shared Workspace
        ↓

IDENTIFY
Market Entry & Opportunity Intelligence
        ↓
        ├──────── Buyer / End Customer ───────→ PRIORITIZE
        │                                      ↓
        │                                   ENGAGE
        │
        └──────── Partner Candidate ─────────→ PARTNER
                                               ↓
                                            ENGAGE

ENGAGE
Business Development Execution
        ↓
Qualified Dialogue → Meeting → Opportunity → Deal Sheet → Mandate Reporting
```

A mixed **Buyers + Partners** mandate can feed both branches. The system does not force every counterparty through one universal funnel.

Cross-module navigation carries only an opaque `mandate_id`. After Private Workspace Access is granted, each app resolves the canonical mandate from the shared workspace.

---


## Commercial Mandate Layer

The shipped applications share a **Commercial Mandate** that can be created once and reused across the full workflow.

The mandate can preserve:

- represented company / client
- origin → target commercial corridor
- product / solution
- commercial objective
- buyer vs partner focus
- target buyer and partner types
- route-to-market hypothesis
- value proposition
- known constraints
- HS / CN / NCM references where available
- target territories and working languages
- success criteria

For cross-border work, the workflow also preserves **Trade & Market Entry Feasibility** verification states covering tariff scenarios, preferential treatment, Ex-Tarifário relevance, rules of origin, import requirements, technical requirements and after-sales needs.

These states organize commercial execution; they are not automatic legal, customs, tariff or technical conclusions.

**Contracts:**

- [Commercial Mandate Contract v1](contracts/commercial-mandate-contract-v1.md)
- [Mandate Workspace Contract v1](contracts/mandate-workspace-contract-v1.md)
- [Trade & Market Entry Feasibility Contract v1](contracts/trade-feasibility-contract-v1.md)
- [Commercial Intelligence Data Contract v1](contracts/commercial-intelligence-data-contract-v1.md)

### Ambrosin Commercial Mandate Workspace

The live applications now use the same workspace model:

- private Supabase-backed mandate persistence
- protected **Private Workspace Access**
- automatic cross-app restoration through `mandate_id`
- active mandate visible before pipeline execution
- stage-aware navigation across IDENTIFY, PRIORITIZE, PARTNER and ENGAGE
- role-aware progression for buyers and partners
- portable JSON fallback
- portable CSV handoffs
- Workspace Snapshot recovery in ENGAGE

The private database stores mandate context and ENGAGE workspace state. Public app users do not receive direct anonymous database access.

This turns the portfolio into a modular Business Development operating workflow rather than four isolated applications.

---


## Current Applications

| Layer | Application | Current Main-Branch Role | Live |
|---|---|---|---|
| **IDENTIFY** | [Opportunity Discovery Intelligence](https://github.com/Eambrosin/opportunity-discovery-intelligence) | Create / restore the mandate, discover buyer and partner universes, preserve evidence and research readiness | [Launch](https://opportunity-discovery-intelligence-eambrosin.streamlit.app/) |
| **PRIORITIZE** | [Counterparty Qualification & Commercial Priority](https://github.com/Eambrosin/lead-qualification-scorer) | Apply configurable ICP and commercial scoring, then route buyers to ENGAGE and partner candidates to PARTNER | [Launch](https://lead-qualification-scorer-eambrosin.streamlit.app/) |
| **PARTNER** | [Route-to-Market & Partner Intelligence](https://github.com/Eambrosin/partnership-opportunity-finder) | Evaluate market access, partner fit, technical / after-sales capability and route-to-market readiness | [Launch](https://partnership-opportunity-finder-eambrosin.streamlit.app/) |
| **ENGAGE** | [Business Development Execution & Outreach](https://github.com/Eambrosin/outreach-sequence-generator) | Execute outreach, follow-up, meetings, opportunity management, deal sheets and mandate reporting | [Launch](https://outreach-sequence-generator-eambrosin.streamlit.app/) |

Tagged releases remain available in the individual repositories; the current main branches include the shared Workspace integration described here.

---


## IDENTIFY — Market Entry & Opportunity Intelligence

**Commercial question:** For this mandate, who could buy or enable market entry, what evidence supports the hypothesis, and what must still be validated?

Current capabilities include:

- Commercial Mandate creation / restoration
- Trade & Market Entry Feasibility states
- configurable sector / market profiles
- mandate-aware public-web discovery
- localized search archetypes
- editorial / research-page holdback
- buyer vs partner role classification
- Account Opportunity
- Qualification Readiness
- account enrichment
- public decision-maker / contact validation
- territory and field-sales intelligence
- evidence gaps and next-best commercial action
- buyer handoff to PRIORITIZE
- partner handoff to PARTNER
- execution continuity into ENGAGE

**Repository:** [opportunity-discovery-intelligence](https://github.com/Eambrosin/opportunity-discovery-intelligence)  
**Live App:** [Launch IDENTIFY](https://opportunity-discovery-intelligence-eambrosin.streamlit.app/)

---


## PRIORITIZE — Counterparty Qualification & Commercial Priority

**Commercial question:** Which counterparties matter most to this mandate, why, what is still unknown and where should each one go next?

Current capabilities include:

- saved Commercial Mandate restoration before pipeline upload
- configurable ICP presets
- weighted, deterministic commercial scoring
- upstream-fit context
- explainable score breakdown
- priority tiers
- company-size / region / industry / value / engagement logic
- qualification and readiness context
- optional AI-assisted interpretation
- role-aware routing:
  - qualified buyers → ENGAGE
  - partner candidates → PARTNER
  - mixed mandates → both paths as appropriate

**Repository:** [lead-qualification-scorer](https://github.com/Eambrosin/lead-qualification-scorer)  
**Live App:** [Launch PRIORITIZE](https://lead-qualification-scorer-eambrosin.streamlit.app/)

---


## ENGAGE — Business Development Execution & Outreach

**Commercial question:** How should we approach the counterparty, progress the dialogue, capture what we learn and advance a qualified opportunity?

Current capabilities include:

- shared mandate restoration
- qualified buyer / partner pipeline intake
- mandate-safe behavior: no demo pipeline is mixed into an active mandate
- adaptive channel and cadence logic
- multilingual qualification-first outreach
- deterministic fallback generation
- optional AI-assisted copy
- executive and territory execution views
- field-day planning and visit feedback
- Business Development Execution Log
- response / meeting / next-action tracking
- Commercial Deal Sheet
- mandate funnel and client-ready reporting
- portable Workspace Snapshot recovery

**Repository:** [outreach-sequence-generator](https://github.com/Eambrosin/outreach-sequence-generator)  
**Live App:** [Launch ENGAGE](https://outreach-sequence-generator-eambrosin.streamlit.app/)

---


## PARTNER — Route-to-Market & Partner Intelligence

**Commercial question:** Which partners can create credible market access and execution capability for this mandate, and what relationship model makes sense?

Current capabilities include:

- shared mandate restoration
- mandate-safe behavior: no demo partner data is mixed into an active mandate
- configurable partnership strategy
- explainable weighted scoring
- strategic-fit and market-access assessment
- relationship-strength signals
- partner-type fit
- Route-to-Market Readiness
- customer-base and geographic-coverage validation
- import capability
- technical service and after-sales capability
- installation / commissioning and field-service capability
- financial capacity and management commitment
- exclusivity / competing-representation validation
- explicit due-diligence gaps
- ENGAGE handoff under the same mandate

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
- [Mandate Workspace Contract v1](contracts/mandate-workspace-contract-v1.md)

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
- opaque `mandate_id` cross-app continuity
- private workspace persistence
- ENGAGE Workspace Snapshot recovery

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
- Supabase / PostgREST for the private shared workspace
- public-web research APIs such as Tavily
- optional LLM APIs
- GitHub Actions
- automated tests and secret scanning

The architecture deliberately separates:

```text
public Streamlit interface
        ↓
Private Workspace Access
        ↓
server-side workspace credentials
        ↓
Supabase Commercial Mandate / Workspace persistence
```

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
