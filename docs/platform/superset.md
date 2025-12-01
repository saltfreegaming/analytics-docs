# Apache Superset

Apache Superset houses long-term behavioral analytics for SFG. Because Superset configuration is not fully managed via IaC, documentation is the control plane for dashboards, datasets, and access.

## Scope of Documentation
- **Dashboards**: Purpose, audience, KPIs, and links to charts.
- **Charts**: Query logic, filters, and expected behavior.
- **Datasets**: Source tables, refresh cadence, owner, and sensitivity.
- **Permissions**: Roles and datasource access rules.

## Authoring Best Practices
- Align every dashboard with a phase (minimum/operational/acceptable/exceptional) and iteration status.
- Store SQL for custom queries in version control or paste into documentation with context and parameter notes.
- Reference Discord Gateway API events used (e.g., `MESSAGE_CREATE`, `VOICE_STATE_UPDATE`) to clarify lineage.
- Capture data validation steps comparing Superset to Grafana logs when relevant.

## Deployment Notes
- Superset content changes must be documented before publishing.
- Use the [Dashboard Documentation Template](../templates-and-checklists/dashboard-template.md) for each dashboard and chart.
- Link Grafana panels when they serve as operational counterparts to Superset views.
