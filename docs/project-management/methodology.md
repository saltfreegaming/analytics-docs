# Delivery Methodology

SFG adopts **Agile with a Kanban flow** optimized for analytics and documentation. Work items flow continuously while respecting clear Definition of Ready and Definition of Done.

## How to Use
1. **Backlog**: Capture ideas, dashboard requests, and data questions as tickets. Include links to the [dashboard template](../templates-and-checklists/dashboard-template.md) for any visualization work.
2. **Prioritize**: The Business Owner orders the backlog weekly based on player impact and data availability.
3. **Design**: The Analytics Engineer drafts requirements and validation steps. Small spikes validate Discord Gateway API coverage when needed.
4. **Build**: Implement Superset charts/SQL, update documentation, and open PRs referencing the relevant checklist.
5. **Test & Review**: Peer review SQL and narrative; validate numbers against trusted sources or Grafana logs.
6. **Deploy**: Merge when the [Release Checklist](../templates-and-checklists/release-checklist.md) is green. GitHub Actions will rebuild and deploy docs.

### Swimlanes
- **Product Discovery**: Exploratory analysis, Discord event mapping, stakeholder interviews.
- **Delivery**: Dashboards, data models, tests, and doc updates.
- **Maintenance**: Bug fixes, data quality issues, access changes.

### Metrics
- Lead time from idea to dashboard publication.
- % of dashboards with complete documentation.
- Freshness of Superset datasets compared to Discord event timestamps.
