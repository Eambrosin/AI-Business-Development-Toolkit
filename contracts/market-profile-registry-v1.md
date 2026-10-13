# Market Profile Registry — v1.0

The portfolio uses stable `market_profile_id` values so the same commercial segment can be recognized across IDENTIFY, PRIORITIZE, ENGAGE and PARTNER.

| Profile ID | Display Segment | Typical Use |
|---|---|---|
| `photovoltaic_energy_consumers` | Fotovoltaico — High-Energy C&I | Energy-consuming commercial / industrial end customers |
| `industrial_machinery_brazil` | Machinery & Equipment — Brazil | Brazilian industrial end buyers; partner search can be activated by mandate |
| `specialty_coffee_europe` | Specialty Coffee — Europe | European importers, roasters and green-coffee buyers |
| `renewable_energy` | Renewable Energy | Legacy / generic renewable-energy compatibility |
| `agribusiness` | Agribusiness | Importers, distributors, processors, traders |
| `logistics_trade` | Logistics & Trade | Freight, customs, shipping, trade services |
| `fintech` | Fintech | Payments, platforms, partnership-led growth |
| `real_estate` | Real Estate | Developers, brokerages, investment/advisory |
| `government_public_sector` | Government / Public Sector | Procurement, institutional and B2G opportunities |
| `medical_aesthetics` | Medical Aesthetics | Clinics, physicians, dermatology, plastic surgery, eligible aesthetic professionals |
| `custom` | Custom | User-defined market profile |

## Photovoltaic C&I safeguards

The `photovoltaic_energy_consumers` profile is designed to discover potential **end customers**, not photovoltaic suppliers.

Typical public signals include industrial production, refrigeration, cold storage, logistics, GDO, hospitality, healthcare, data centers and other operationally energy-intensive activities.

Installer, distributor, wholesaler and photovoltaic EPC signals are treated as non-target evidence.

A discovery match does **not** establish verified electricity consumption or technical feasibility. Load profile, available surface, self-consumption potential, grid constraints, investment timing and technical design remain qualification questions.

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


## Territory profiles

Territory profiles are a separate configuration layer from market profiles.

Current profile:

```text
territory_profile_id: it_north_medical_aesthetics
market_profile_id: medical_aesthetics
country: Italy
regions:
  - Lombardia
  - Veneto
  - Trentino-Alto Adige
```

The current territory profile supports province/city commercial clusters and bilingual Italian/German search context for Bolzano / Bozen and Südtirol.

## Vendor / commercial profiles

Vendor profiles are optional commercial-context layers.

Current profile:

```text
vendor_profile_id: deleo_north_italy
market_profile_id: medical_aesthetics
territory_profile_id: it_north_medical_aesthetics
```

Vendor profiles can contribute discussion themes, technology evidence terms and support-model context. They must not automatically decide product suitability, professional eligibility or clinical appropriateness.
