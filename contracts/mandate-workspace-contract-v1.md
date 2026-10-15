# Commercial Mandate Workspace Contract v1

The Commercial Mandate Workspace is the persistence and execution layer that connects the four Ambrosin Commercial Intelligence modules without creating a fifth standalone product.

## Workflow

```text
COMMERCIAL MANDATE
        ↓
IDENTIFY
Market Entry & Opportunity Intelligence
        ↓
PRIORITIZE / PARTNER
Counterparty Qualification / Route-to-Market Intelligence
        ↓
ENGAGE
Business Development Execution
        ↓
ACTIVE OPPORTUNITY
        ↓
COMMERCIAL DEAL SHEET
        ↓
MANDATE REPORTING
```

## Workspace identity

Every persistent workspace is anchored to one stable:

```text
mandate_id
```

The same mandate identifier should travel with downstream pipeline rows, execution updates and deal sheets.

A persistent workspace may use:

```text
workspace_id = "workspace_" + mandate_id
```

for one current operational snapshot per mandate.

## Workspace Snapshot schema

Current portable schema version:

```text
workspace_snapshot_schema_version = "1.0"
```

Top-level fields:

| Field | Purpose |
|---|---|
| workspace_snapshot_schema_version | Contract version |
| exported_at_utc | Snapshot export timestamp |
| source_stage | Current originating module |
| source_name | Human-readable pipeline/source name |
| mandate | Canonical Commercial Mandate payload |
| pipeline | Current counterparty pipeline |
| execution_updates | Business Development Execution records |
| deal_sheets | Commercial Deal Sheets |
| field_visit_feedback | Structured field-visit feedback |

## Operational principle

The Workspace stores **recorded commercial activity**.

It must not silently convert:

- hypotheses into facts
- unknown information into verified information
- internal scoring into buyer intent
- missing trade/regulatory validation into approval
- indicative deal value into committed revenue

The evidence-aware principle remains:

```text
Unknown stays unknown until validated.
```

## Next Action Queue

Execution records may carry:

- company_name
- opportunity_stage
- response_status
- next_action
- next_action_date
- upstream_tier

The operational workspace can derive:

- Overdue
- Due Today
- Upcoming
- Unscheduled

and a working priority such as:

- High
- Medium
- Normal

These are workflow aids, not autonomous sales decisions.

## Cross-module handoff

Once a mandate is persisted, the shared navigation may transport the opaque `mandate_id` between modules as a URL query parameter.

The receiving module resolves the canonical mandate from the private backend after workspace access is authorized.

The transport URL must not contain:

- database credentials
- the private Workspace Access Token
- client confidential data
- commercial notes
- deal terms

Portable JSON remains the offline / fallback handoff.

## Persistence model

Two logical entities are sufficient for the current Ambrosin internal-use phase:

### Commercial Mandate

Stores the canonical client / corridor / product / objective context.

Primary key:

```text
mandate_id
```

### Commercial Workspace

Stores the current operational snapshot for the mandate.

Primary key:

```text
workspace_id
```

Foreign key:

```text
mandate_id → Commercial Mandate
```

## Security boundary

Workspace records may contain commercially sensitive information.

The current implementation is intended for **private Ambrosin internal use**, not as a public multi-tenant SaaS.

Recommended controls:

- private database
- server-side secrets only
- Row Level Security enabled
- no anonymous public read/write policies
- privileged database key never committed to GitHub
- a separate private Workspace Access Token before cloud read/write is enabled
- the Workspace Access Token never placed in shared URLs
- portable snapshots treated as confidential mandate files

A future client portal requires authenticated users, mandate ownership and explicit tenant-level RLS policies.

## Module responsibilities

### IDENTIFY

Creates or receives the Commercial Mandate and generates researched counterparties.

### PRIORITIZE

Evaluates buyer / counterparty relevance to the mandate.

### PARTNER

Evaluates route-to-market, distributor and technical-service readiness.

### ENGAGE

Owns ongoing execution, next actions, meetings, active opportunities, deal sheets and reporting.

The persistent Mandate Workspace is therefore an operational layer around the modules, not a replacement for them.
