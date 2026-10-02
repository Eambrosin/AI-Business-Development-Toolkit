![Global Operations](assets/banners/global-operation.jpg)

# AI Business Development Toolkit

### AI-Assisted Commercial Intelligence | Business Development | GTM | Strategic Partnerships | International Expansion

![Commercial Intelligence](https://img.shields.io/badge/Commercial%20Intelligence-Ecosystem-1f6feb)
![Discovery](https://img.shields.io/badge/IDENTIFY-Live-success)
![Lead Qualification](https://img.shields.io/badge/PRIORITIZE-v2.0.0-success)
![Adaptive Outreach](https://img.shields.io/badge/ENGAGE-v2.1.0-success)
![Partnership Intelligence](https://img.shields.io/badge/PARTNER-v2.0.0-success)
![Market Expansion](https://img.shields.io/badge/ROADMAP-Market%20Expansion-orange)

A practical portfolio of AI-assisted tools, strategic frameworks and commercial intelligence systems designed to support Business Development, Go-to-Market execution, strategic partnerships and international market expansion.

This repository serves as the central hub connecting a growing ecosystem of applications and frameworks focused on practical commercial decision-making.

The objective is not to build technology for technology's sake.

The objective is to use AI, structured data and commercial strategy to answer practical business questions:

* Which opportunities deserve attention?
* Where should commercial resources be allocated?
* How should organizations approach and develop opportunities?
* Which partners offer the strongest strategic fit?
* Which markets should organizations enter?
* What should the next commercial action be?

---

## Commercial Intelligence Lifecycle

The portfolio is structured around five stages of the Business Development and international growth lifecycle:

### Identify → Prioritize → Engage, with a parallel Partner track

| Stage          | System                    | Commercial Purpose                                           |
| -------------- | ------------------------- | ------------------------------------------------------------ |
| **Identify**   | Opportunity Discovery Intelligence | Discover and screen target accounts using market-specific criteria and evidence |
| **Prioritize** | Revenue Prioritization    | Determine where commercial resources should be allocated     |
| **Engage**     | Outreach Intelligence     | Structure outreach, follow-up and opportunity development    |
| **Partner**    | Partnership Intelligence  | Identify and evaluate strategic partners and ecosystems      |
| **Roadmap**    | Market Expansion Intelligence | Future layer for structured international expansion decisions |

Together, these systems form an evolving AI-assisted Commercial Intelligence ecosystem.

---

## Current Product Status

The toolkit is evolving from a collection of Business Development experiments into an integrated Commercial Intelligence ecosystem.

### 🔎 IDENTIFY — Opportunity Discovery Intelligence

**Status:** Live standalone application — v1.0

A configurable target-account discovery application for adapting lead generation to a client-specific market profile.

Core capabilities include:

- Multi-segment market profiles plus fully custom configuration
- Target industry configuration
- Country and region targeting
- Business-model filters
- Required and excluded keywords
- Company-size preferences
- Sample, CSV and optional public-web discovery modes
- Explainable Discovery Score
- Separate Confidence Score
- Evidence URLs and source snippets
- Unknown-information tracking
- Recommended next actions
- Qualification handoff template
- Optional evidence-aware AI research brief
- Public LinkedIn contact intelligence through indexed web results
- Selective Account Enrichment for website, public business contacts, address and fit evidence
- Account Data Completeness with source-preserving evidence
- Direct handoffs to PRIORITIZE and ENGAGE

The application intentionally separates **discovery** from **formal qualification**. Unknown information is surfaced for validation instead of being silently treated as fact.

[View Repository](https://github.com/Eambrosin/opportunity-discovery-intelligence)

[Launch Application](https://opportunity-discovery-intelligence-eambrosin.streamlit.app/)

> **Demo affiliation note:** the DELEO commercial-program preset is a portfolio demonstration built from publicly available information. The project is not affiliated with, sponsored by or endorsed by DELEO.


#### North Italy Territory Intelligence

Medical Aesthetics now includes a territory layer for **Lombardia · Veneto · Trentino-Alto Adige**, with province/city clusters, technology evidence, selective account enrichment, public-contact discovery, Account Opportunity Score, Contact Readiness and territory execution handoffs.

A DELEO-specific commercial profile can be activated as an optional evidence/discussion layer without changing the generic discovery engine.


---

### ✅ PRIORITIZE — Lead Qualification & Revenue Prioritization

**Status:** Shipped — v2.0.0

A configurable Commercial Intelligence platform for evaluating pipeline opportunities against an Ideal Customer Profile.

Core capabilities include:

- Configurable ICP
- Region Fit
- Industry Fit
- Company Size Fit
- Deal Value assessment
- Engagement scoring
- Explainable commercial scoring
- Priority tiers
- Recommended commercial actions
- Executive pipeline prioritization
- Optional AI-assisted account intelligence

[View Repository](https://github.com/Eambrosin/lead-qualification-scorer)

[Launch Application](https://lead-qualification-scorer-eambrosin.streamlit.app/)

---

### ✅ ENGAGE — Adaptive Outreach Intelligence

**Status:** Shipped — v2.0.0

An adaptive Commercial Intelligence platform that converts qualification context into prioritized, multilingual outreach execution.

Core capabilities include:

- Commercial Intelligence Mode
- Standard Outreach Mode
- Adaptive commercial priority
- Dynamic outreach cadence
- Multilingual communication
- Country-based channel strategy
- Prospecting and Post-Proposal workflows
- Revenue At Risk visibility
- Commercial Decision Support
- Deterministic local fallback
- Optional AI-assisted message generation

The application can directly consume prioritized pipeline exports from the Lead Qualification platform.

[View Repository](https://github.com/Eambrosin/outreach-sequence-generator)

[Launch Application](https://outreach-sequence-generator-eambrosin.streamlit.app/)

---

### 🤝 PARTNER — Partnership Intelligence

**Status:** Shipped — v2.0.0

Identifies, scores and prioritizes strategic partnership opportunities.

[View Repository](https://github.com/Eambrosin/partnership-opportunity-finder)

---

### 🗺️ ROADMAP — Market Expansion Intelligence

**Status:** Roadmap / not presented as a shipped product

A future layer for structured international market-entry decisions. It remains outside the shipped product set until it reaches the same implementation, testing and demo standard as IDENTIFY, PRIORITIZE, ENGAGE and PARTNER.

---

## Integrated Commercial Intelligence Architecture

The portfolio now uses **two coordinated commercial tracks** rather than forcing every opportunity through one linear funnel.

```text
ACCOUNT DEVELOPMENT

IDENTIFY
Opportunity Discovery Intelligence
+ Account Enrichment
        ↓
PRIORITIZE
Lead Qualification & Revenue Prioritization
        ↓
ENGAGE
Adaptive Outreach Intelligence


PARTNERSHIP DEVELOPMENT

IDENTIFY / EXISTING PARTNER UNIVERSE
        ↓
PARTNER
Partnership Intelligence
        ↓
ENGAGE
Adaptive Partner Outreach


FUTURE ROADMAP
        ↓
MARKET EXPANSION INTELLIGENCE
```

The applications exchange portable CSV handoffs with shared metadata such as `schema_version`, `source_stage` and `market_profile_id`.

**Shared contracts**
- [Commercial Intelligence Data Contract v1](contracts/commercial-intelligence-data-contract-v1.md)
- [Market Profile Registry v1](contracts/market-profile-registry-v1.md)

Canonical market profiles currently include Renewable Energy, Agribusiness, Logistics & Trade, Fintech, Real Estate, Government / Public Sector and Medical Aesthetics, while preserving a fully custom mode.

---

## Featured Applications

### 🎯 Lead Qualification & Revenue Prioritization

**Role in the ecosystem:** `Identify → Prioritize`

AI-assisted commercial intelligence platform designed to help Business Development teams identify which accounts and opportunities deserve immediate attention.

#### Core Capabilities

* Lead Scoring
* Tier Classification
* Revenue Prioritization
* Executive Account Dashboard
* Lead Intelligence Workspace
* AI Account Intelligence
* AI Outreach Generation
* GTM Recommendations

#### Business Problem

Commercial teams frequently have more opportunities than they can effectively pursue.

This application helps structure prioritization so resources can be focused on higher-potential accounts and opportunities.

#### Live Application

[Launch Lead Qualification & Revenue Prioritization](https://lead-qualification-scorer-eambrosin.streamlit.app/)

#### Repository

[View lead-qualification-scorer](https://github.com/Eambrosin/lead-qualification-scorer)

---

### ✉️ Outreach Intelligence

**Role in the ecosystem:** `Engage`

AI-assisted outreach and follow-up platform designed to support structured commercial engagement and improve Business Development execution.

#### Core Capabilities

* Executive Outreach Dashboard
* Follow-Up Prioritization
* Business Development Intelligence
* AI Outreach Generation
* Revenue Risk Analysis
* Commercial Opportunity Assessment
* Multi-Step Follow-Up Sequences

#### Business Problem

Strong opportunities can be lost through inconsistent outreach, poor prioritization or weak follow-up discipline.

The application combines commercial intelligence with AI-assisted communication to help teams structure account engagement.

#### Live Application

[Launch Outreach Intelligence](https://outreach-sequence-generator-eambrosin.streamlit.app/)

#### Repository

[View outreach-sequence-generator](https://github.com/Eambrosin/outreach-sequence-generator)

---

### 🤝 Partnership Opportunity Finder

**Role in the ecosystem:** `Partner`

Explainable decision-support platform for identifying, evaluating and prioritizing strategic partnership opportunities.

#### Core Capabilities

* Partnership Fit Scoring
* Executive Partnership Dashboard
* Opportunity Heatmap
* Regional Expansion Dashboard
* Partner Portfolio Analysis
* Executive Recommendation Center
* Partnership Intelligence Workspace

#### Business Problem

Organizations evaluating multiple potential partners often lack a consistent methodology for comparing strategic fit, commercial potential and expansion relevance.

This system provides a structured framework for partnership prioritization and strategic decision-making.

#### Live Application

[Launch Partnership Opportunity Finder](https://partnership-opportunity-finder-eambrosin.streamlit.app/)

#### Repository

[View partnership-opportunity-finder](https://github.com/Eambrosin/partnership-opportunity-finder)

---

## 🌍 In Development

### Global Market Entry Intelligence

**Role in the ecosystem:** `Expand`

A decision-support system designed to help organizations evaluate international expansion opportunities and structure market-entry strategy.

The project will combine commercial, strategic, regulatory and operational factors into a structured international expansion framework.

#### Planned Capabilities

* Market Attractiveness Assessment
* Commercial Readiness Analysis
* Market Entry Barrier Mapping
* Partner Dependency Assessment
* Channel Strategy Analysis
* Localization Requirements
* GTM Strategy Recommendations
* Expansion Risk Analysis
* Market Prioritization
* 90-Day Market Entry Action Plan

#### Core Business Question

**Where should an organization expand next, and what commercial strategy should it use to enter that market?**

Initial use cases will focus on cross-border commercial analysis involving Europe, Brazil, LATAM and MENA.

---

## Strategic Frameworks & Playbooks

Technology alone does not create effective Business Development execution.

The ecosystem is supported by strategic frameworks covering areas such as:

* Lead Qualification
* Account Prioritization
* GTM Planning
* Partnership Development
* International Market Entry
* Commercial Opportunity Assessment
* Revenue Operations
* Cross-Border Business Development

Supporting frameworks are maintained in:

[View BD Frameworks & Playbooks](https://github.com/Eambrosin/bd-frameworks-and-playbooks)

---

## Commercial Intelligence Architecture

The broader portfolio is designed around a simple principle:

### Data → Intelligence → Prioritization → Action

Raw commercial information only becomes valuable when it supports a decision.

The systems in this portfolio are therefore designed to move from information toward actionable commercial recommendations.

### Data

Accounts, opportunities, markets, partners and commercial variables.

### Intelligence

Structured assessment of opportunity quality, fit, risk and strategic relevance.

### Prioritization

Determination of where time, capital and commercial resources should be allocated.

### Action

Outreach, partnership development, GTM execution or market-entry decisions.

---

## Strategic Focus Areas

The portfolio currently focuses on:

* International Business Development
* Strategic Partnerships
* Go-to-Market Strategy
* Revenue Operations
* Commercial Intelligence
* International Market Expansion
* Market Entry Strategy
* Sales Prioritization
* Partnership Ecosystem Development
* AI-Assisted Commercial Decision-Making
* AI Workflow Automation

---

## International Expansion Intelligence

Cross-border growth requires more than market-size analysis.

Commercial expansion decisions may involve:

* Market attractiveness
* Customer demand
* Competitive positioning
* Channel availability
* Partnership ecosystems
* Regulatory requirements
* Institutional considerations
* Localization requirements
* Geopolitical exposure
* Operational feasibility

These factors will increasingly be integrated into the Market Entry Intelligence layer of the portfolio.

Geopolitical and regulatory analysis are treated as supporting dimensions of international commercial strategy rather than standalone objectives.

---

## Executive Intelligence Prototypes

The following visual prototypes explore how complex commercial and international expansion information can be translated into executive decision-support interfaces.

### Global Expansion Intelligence Dashboard

**Type:** Strategic Concept Dashboard

A conceptual executive dashboard focused on international market prioritization, geopolitical context, strategic partnerships and commercial expansion opportunities.

![Global Expansion Intelligence Dashboard](assets/screenshots/global-expansion-dashboard.png)

---

### AI Commercial Operations Dashboard

**Type:** Commercial Intelligence Prototype

A conceptual executive interface focused on lead qualification, commercial pipeline intelligence, revenue operations, partnership analytics and workflow automation.

![AI Commercial Operations Dashboard](assets/screenshots/ai-commercial-operations-dashboard.png)

---

### Geopolitical Risk Intelligence Matrix

**Type:** Strategic Analysis Prototype

A visual framework exploring how geopolitical, regulatory and institutional factors can be incorporated into international expansion analysis.

![Geopolitical Risk Intelligence Matrix](assets/screenshots/geopolitical-risk-intelligence-matrix.png)

---

### International Expansion Strategic Framework

**Type:** Strategic Framework

A structured model for evaluating international expansion through market intelligence, regulatory analysis, partnerships, operational execution and continuous optimization.

![International Expansion Strategic Framework](assets/screenshots/international-expansion-strategic-framework.png)

---

## Technology

The current applications and prototypes use technologies including:

* Python
* Streamlit
* Pandas
* Plotly
* OpenAI API
* Data Analytics
* AI-Assisted Workflows

Technology is treated as an enabler for commercial decision-making rather than the end objective of the portfolio.

---

## Portfolio Structure

This repository acts as the strategic hub connecting the main components of the ecosystem.

### Profile

[Eduardo Ambrosin — GitHub Profile](https://github.com/Eambrosin)

### Applications

[Lead Qualification & Revenue Prioritization](https://github.com/Eambrosin/lead-qualification-scorer)

[Outreach Intelligence](https://github.com/Eambrosin/outreach-sequence-generator)

[Partnership Opportunity Finder](https://github.com/Eambrosin/partnership-opportunity-finder)

### Knowledge Base

[BD Frameworks & Playbooks](https://github.com/Eambrosin/bd-frameworks-and-playbooks)

### In Development

**Global Market Entry Intelligence**

---

## Development Roadmap

The portfolio is actively evolving from standalone applications toward a connected Commercial Intelligence ecosystem.

Current development priorities include:

* Configurable ICP and opportunity-scoring models
* Deeper revenue prioritization
* Multilingual outreach workflows
* Partnership portfolio intelligence
* International market-entry analysis
* Cross-border commercial readiness
* Integrated Commercial Intelligence dashboards

For the detailed development roadmap:

[View ROADMAP.md](ROADMAP.md)

---

## Professional Perspective

This portfolio reflects the intersection of international Business Development, commercial strategy, strategic partnerships, market expansion and AI-assisted decision-making.

The central idea is simple:

**AI should help commercial professionals make better decisions, not replace commercial judgment.**

The projects therefore focus on practical questions faced by Business Development and international growth teams:

**Where is the opportunity?**

**How valuable is it?**

**What should be prioritized?**

**How should we engage?**

**Who should we partner with?**

**Where should we expand?**

**What should we do next?**

---

## Connect

### Professional Website

🌐 [ambrosinlegaltrade.com](https://www.ambrosinlegaltrade.com/)

### LinkedIn

💼 [linkedin.com/in/eduardoambrosin](https://www.linkedin.com/in/eduardoambrosin/)

### GitHub

💻 [github.com/Eambrosin](https://github.com/Eambrosin)
