# Dashboard Documentation Template

Use this template for every Apache Superset dashboard. Copy the sections and fill them out in a dedicated page under `docs/platform/` or a subfolder.

## Overview
- **Dashboard name**:
- **Owner**:
- **Audience**:
- **Phase**: minimum / operational / acceptable / exceptional
- **Iteration status**: design / build / test / ready
- **Related Grafana panels**:

## Purpose & Questions
- What decision does this dashboard support?
- Key business questions and success metrics.

## Data Sources
- Superset dataset(s) and schemas.
- Discord Gateway API events utilized (e.g., `MESSAGE_CREATE`, `VOICE_STATE_UPDATE`).
- Refresh cadence and retention window.

## KPI Definitions
- KPI name, formula, and filters.
- Dimensionality (e.g., by channel, role, region).
- Acceptance criteria and validation steps.

## Visuals & Interactions
- List charts with titles and links.
- Default filters, drill paths, and expected user flows.
- Accessibility considerations (color, labeling).

## Security & Permissions
- Roles with access.
- Sensitivity level (public/internal/confidential).

## Change Log
- Date, change description, and reviewer.

## Open Questions & Next Steps
- Pending data gaps or feature requests.
- Experiments or A/B tests to run in the next phase.
