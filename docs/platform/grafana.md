# Grafana Logging

Grafana captures short-term, operational telemetry for SFG. Use it for debugging ingestion issues and validating Superset calculations.

## Usage
- Monitor ingestion lag and error rates for Discord data pipelines.
- Trace anomalies seen in Superset back to raw events and logs.
- Document alert policies and on-call expectations for critical pipelines.

## Documentation Pointers
- Note retention windows and sampling strategies for each Grafana datasource.
- Link Grafana panels to their related Superset dashboards to clarify scope (operational vs. behavioral).
- Record troubleshooting runbooks when recurrent issues surface.
