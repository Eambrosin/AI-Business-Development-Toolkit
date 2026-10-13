# Commercial Mandate Contract — v1.0

The Commercial Mandate is the shared project context across the Commercial Intelligence portfolio.

It exists to answer one question before any account, partner or outreach decision is made:

> **What commercial mandate are we executing, for whom, between which markets, and what outcome defines success?**

The mandate is created upstream and preserved across IDENTIFY, PRIORITIZE, PARTNER and ENGAGE.

## Core fields

```text
mandate_schema_version
mandate_id
mandate_name
mandate_status
mandate_client
mandate_corridor
mandate_origin_market
mandate_target_market
mandate_product
mandate_product_category
mandate_commercial_objective
mandate_target_buyer_types
mandate_target_partner_types
mandate_route_to_market
mandate_value_proposition
mandate_known_constraints
mandate_hs_code
mandate_cn_code
mandate_ncm_code
mandate_target_territories
mandate_working_languages
mandate_success_criteria
```

## Typical Ambrosin corridors

```text
Europe → Brazil / Mercosur
Brazil / Mercosur → Europe
Italy → Brazil
Brazil → Italy
Europe → Mercosur
Other international corridor
```

The corridor is commercial context, not a legal or customs conclusion.

## Example

```text
mandate_name:
Italian Packaging Machinery → Brazil

mandate_client:
Example Manufacturer

mandate_corridor:
Italy → Brazil

mandate_origin_market:
Italy

mandate_target_market:
Brazil

mandate_product:
Automatic packaging machinery

mandate_product_category:
Industrial Machinery

mandate_commercial_objective:
Develop qualified Brazilian end customers and validate a local
commercial / technical route to market

mandate_target_buyer_types:
Food manufacturers, beverage manufacturers, packaging companies

mandate_target_partner_types:
Distributor, sales agent, technical service partner

mandate_route_to_market:
Direct manufacturer sales supported by a local commercial /
technical partner

mandate_success_criteria:
Qualified meetings, active opportunities, quotations and sale
```

## Stage behavior

### IDENTIFY

Creates or receives the mandate and uses it to frame:

- target-market discovery
- buyer universe
- partner universe
- sector / product context
- qualification questions
- public evidence

### PRIORITIZE

Preserves the mandate while evaluating:

- commercial attractiveness
- qualification completeness
- relative priority
- next commercial action

### PARTNER

Preserves the mandate while evaluating:

- route-to-market contribution
- market access
- execution feasibility
- partner model
- due-diligence questions

### ENGAGE

Preserves the mandate while converting context into:

- stakeholder strategy
- outreach
- qualification dialogue
- follow-up
- next action

## Design rules

1. **One mandate can contain many counterparties.**
2. **Mandate context must survive CSV handoffs.**
3. **Unknown trade / regulatory information remains unknown.**
4. **HS, CN and NCM fields are references to validate, not automatic classifications.**
5. **A target account score is relative to the mandate, not a claim of purchase intent.**
6. **Buyer and partner roles must remain distinguishable.**
7. **The mandate should support measurable reporting without inventing results.**
