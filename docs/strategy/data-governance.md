# Data Governance

SFG balances agility with responsible handling of member data. Governance practices ensure Superset content is trustworthy and appropriately limited.

## Principles
- **Transparency**: Document assumptions, filters, and definitions for every dashboard.
- **Least privilege**: Grant Superset and Grafana access based on role; avoid broad admin rights.
- **Retention-aware**: Grafana stores short-lived diagnostic logs; Superset retains long-term behavioral data. Document retention windows alongside datasets.
- **Reproducibility**: Store SQL queries and calculations in version control when feasible; link to them from dashboard docs.

## Controls
- Maintain a **dataset inventory** with owners, refresh cadence, and source system.
- Track **data lineage** from Discord Gateway API events → staging → curated tables → dashboards.
- Use **data quality checks** (null rates, freshness, row counts) and record outcomes in release notes.
- Tag dashboards with **sensitivity** (public/internal/confidential) to align permissions.

## Collaboration
- The Analytics Engineer authors technical details; the Business Owner validates KPIs and narrative context.
- Every change request should cite the relevant dashboard documentation page and expected business impact.
