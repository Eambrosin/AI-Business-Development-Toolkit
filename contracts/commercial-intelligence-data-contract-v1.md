# Commercial Intelligence Data Contract — v1.0

This document defines the shared handoff contract across the standalone Commercial Intelligence applications.

The objective is **integration without tight coupling**: every app remains independently deployable, but exports predictable metadata that downstream apps can preserve and understand.

## Core metadata

| Field | Purpose |
|---|---|
| `schema_version` | Version of the shared handoff contract |
| `source_stage` | Stage that produced the current export: IDENTIFY, PRIORITIZE, ENGAGE or PARTNER |
| `market_profile_id` | Stable market-segment identifier shared across apps |

Current canonical profile IDs:

- `renewable_energy`
- `agribusiness`
- `logistics_trade`
- `fintech`
- `real_estate`
- `government_public_sector`
- `medical_aesthetics`
- `custom`

## Account fields

Common account-level fields include:

```text
company_name
country
region
industry
company_size
business_model
source_url
source_domain
discovery_score
confidence
professional_setting
```

Apps should preserve unknown fields rather than silently deleting them.

## Public contact fields

When public professional-profile evidence is available:

```text
contact_name
contact_headline
linkedin_url
outreach_angle
professional_setting
```

These fields represent **publicly indexed evidence or workflow context**, not guaranteed-current identity data. Current role and company should be verified before outreach.

## Qualification fields

```text
estimated_deal_value_usd
engagement_signal
score
tier
recommended_action
score_rationale
```

A discovery-stage placeholder value must not be interpreted as verified commercial information. For example, a deal value of `0` in an IDENTIFY handoff can mean **unknown / not yet qualified**, not a confirmed zero-value opportunity.

## Partnership fields

```text
partner_name
partner_type
strategic_goal
market_overlap
execution_complexity
relationship_signal
partnership_fit_score
partnership_archetype
```

## Recommended stage handoffs

### Account-development path

```text
IDENTIFY
Opportunity Discovery
        ↓
PRIORITIZE
Lead Qualification
        ↓
ENGAGE
Adaptive Outreach
```

### Partnership-development path

```text
IDENTIFY or Existing Partner Universe
        ↓
PARTNER
Partnership Intelligence
        ↓
ENGAGE
Adaptive Partner Outreach
```

Partnership analysis is therefore a **parallel commercial track**, not a mandatory downstream step for every sales lead.

### Expansion layer

```text
Account + Partnership + Market Evidence
        ↓
EXPAND
Market Entry / Territory Intelligence
```

## Design rules

1. **Loose coupling:** no app should depend on another app being online.
2. **Stable exports:** CSV remains the portable baseline handoff format.
3. **Preserve metadata:** downstream apps should retain useful upstream fields.
4. **No silent assumptions:** unknown values remain unknown or explicitly flagged.
5. **Explainable scores:** each app owns its scoring logic and does not overwrite upstream scores.
6. **Market profiles configure; engines stay generic:** sector-specific logic belongs in a profile layer whenever possible.
7. **Human verification before outreach:** public-source contact evidence can be stale.
8. **Version the contract:** breaking field changes require a new schema version.
