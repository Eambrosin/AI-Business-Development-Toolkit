# Market Profile Registry — v1.0

The portfolio uses stable `market_profile_id` values so the same commercial segment can be recognized across IDENTIFY, PRIORITIZE, ENGAGE and PARTNER.

| Profile ID | Display Segment | Typical Use |
|---|---|---|
| `renewable_energy` | Renewable Energy | Distributors, EPCs, energy solutions |
| `agribusiness` | Agribusiness | Importers, distributors, processors, traders |
| `logistics_trade` | Logistics & Trade | Freight, customs, shipping, trade services |
| `fintech` | Fintech | Payments, platforms, partnership-led growth |
| `real_estate` | Real Estate | Developers, brokerages, investment/advisory |
| `government_public_sector` | Government / Public Sector | Procurement, institutional and B2G opportunities |
| `medical_aesthetics` | Medical Aesthetics | Clinics, physicians, dermatology, plastic surgery, eligible aesthetic professionals |
| `custom` | Custom | User-defined market profile |

## Medical Aesthetics safeguards

The `medical_aesthetics` profile can include clinics, physicians, dermatologists, plastic surgeons, clinic managers and aesthetic professionals as discovery candidates.

A discovery match **does not establish product eligibility**.

Where professional scope or device classification matters, the workflow should carry a validation signal such as:

```text
Medical-setting signal observed
Professional/device eligibility to validate
Professional setting unknown
```

This keeps the commercial workflow useful without turning market discovery into an unsupported regulatory or clinical conclusion.

## Profile behavior by app

### IDENTIFY

Profiles configure:

- search archetypes
- positive fit signals
- exclusions
- target geographies
- target account types
- target decision-maker roles

### PRIORITIZE

Profiles inform:

- industry recognition
- ICP choices
- region normalization
- qualification context

The deterministic scoring engine remains configurable by the user.

### ENGAGE

Profiles inform:

- stakeholder suggestions
- domain-specific validation questions
- upstream outreach angles
- language/channel defaults through country profiles

Commercial priority remains driven by qualification context.

### PARTNER

Profiles inform:

- industry alignment
- relevant partner types
- partnership archetypes
- strategic-goal interpretation

Partnership scoring remains deterministic and explainable.
