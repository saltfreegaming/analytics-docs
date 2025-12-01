# Platform Roadmap

SFG's analytics program progresses through four phases. Each phase inherits prior work and runs its own **design → build → test** cycle.

| Phase | Objective | Key Deliverables | Completion Signals |
| --- | --- | --- | --- |
| Minimum | Stand up the baseline documentation and tooling. | MkDocs site, GitHub Actions deploy, initial Superset inventory template, Discord data feed mapped. | Docs build automatically, template used for first dashboard entry. |
| Operational | Enable day-to-day reporting for Dota 2 and Discord engagement. | Core Superset datasets (players, sessions, channel activity), Grafana alert references, weekly release notes. | Project board shows steady throughput; stakeholders review dashboards weekly. |
| Acceptable | Broaden coverage to multi-game analytics and retention insights. | Cross-game cohort analyses, standardized KPI glossary, data quality checks. | KPIs accepted by Business Owner; documentation completeness >80% for dashboards. |
| Exceptional | Optimize for experimentation and longevity. | Experiment design playbook, automated data freshness checks, advanced visual themes. | A/B tests documented; superseded dashboards archived with rationale. |

## Iteration Cadence
- **Design**: Capture requirements in the [dashboard template](../templates-and-checklists/dashboard-template.md) and plan work in the project board.
- **Build**: Implement Superset charts, SQL, and permissions; integrate Discord Gateway API-derived datasets.
- **Test**: Validate data freshness, chart correctness, and accessibility. Record findings in release notes.

## Governance Hooks
- Every phase must tag dashboards with phase metadata in Superset (via tags or naming conventions).
- Retire artifacts by marking them "deprecated" and linking to replacements in documentation.
- Use the [Release Checklist](../templates-and-checklists/release-checklist.md) before publishing dashboard updates.
