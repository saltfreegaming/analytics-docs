# analytics-docs

Project home for the analytics documentation for Salt Free Gaming's BI system. Documentation is authored in Markdown and rendered via MkDocs (Material theme), with static output served through GitHub Pages.

## Structure
- `docs/` – Source Markdown organized by strategy, project-management, platform, data, and templates.
- `static/` – Generated MkDocs site (do not edit manually).
- `mkdocs.yml` – Site configuration and navigation.
- `.github/workflows/` – Automation for building and deploying the site.
- `AGENTS.md` – Guidelines for AI agents contributing to this repository.

## Local Development
1. Install dependencies: `pip install -r requirements.txt`
2. Serve locally: `mkdocs serve` (opens at http://localhost:8000)
3. Build static site: `mkdocs build --clean`

## Deployment
- On pushes to `main`, GitHub Actions build the site into `static/` and deploy the contents to GitHub Pages automatically.

## Documentation Focus
The site covers the end-to-end analytics program for SFG, including Apache Superset dashboards for long-term behavioral analysis, Grafana logging for short-term diagnostics, Discord Gateway API data ingress, and the Agile Kanban delivery methodology used by the Business Owner and Analytics Engineer.
