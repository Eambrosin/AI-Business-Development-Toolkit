# Trade & Market Entry Feasibility Contract — v1.0

This contract defines the portable trade-feasibility context shared across the Commercial Intelligence workflow.

Its purpose is **not** to automate legal, customs, engineering or regulatory conclusions.

Its purpose is to make the verification state explicit before a commercial opportunity is advanced.

## Status vocabulary

Each feasibility dimension uses one of:

```text
Unknown
To Verify
In Review
Verified
Not Applicable
```

## Portable fields

```text
trade_feasibility_schema_version
trade_feasibility_status
trade_tariff_scenario_status
trade_preferential_treatment_status
trade_ex_tarifario_status
trade_rules_of_origin_status
trade_import_requirements_status
trade_technical_requirements_status
trade_after_sales_status
trade_feasibility_notes
trade_specialist_validation_notes
```

## Europe → Brazil use case

For European machinery or equipment entering Brazil, the workflow can organize questions around:

- preliminary HS / NCM reference
- tariff and landed-cost scenario
- potential preferential-treatment eligibility
- potential Ex-Tarifário relevance
- rules of origin
- import / customs requirements
- technical or certification requirements
- after-sales / local service requirements
- issues requiring customs, engineering, regulatory or legal specialist validation

A status of `Verified` should only be used when the relevant evidence or specialist validation supports it.

## Design rules

1. **No automatic entitlement claims.**
2. **NCM / HS references remain subject to validation.**
3. **Ex-Tarifário relevance is separate from EU–Mercosur preferential treatment.**
4. **Preferential treatment depends on product classification, origin and applicable schedules.**
5. **Technical requirements may require qualified engineering or regulatory review.**
6. **The app organizes commercial readiness; it does not issue legal or conformity opinions.**
7. **Unknown remains unknown until validated.**
