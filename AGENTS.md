# AGENTS

- This repository uses MkDocs (Material theme) with `site_dir` set to `static`. Do not place authored Markdown in `static/`; it is generated content.
- Add new documentation inside `docs/` and register it in `mkdocs.yml` navigation.
- Prefer concise section titles and include organizational context for Salt Free Gaming (SFG) when relevant.
- Keep references to dashboards, charts, and data sources descriptive so non-technical stakeholders can follow.
- Avoid try/except around imports.
- Update `README.md` if build or deployment steps change.
- Run `mkdocs build --clean` before committing significant docs or configuration changes.
- GitHub Actions definitions live in `.github/workflows/`; ensure workflows remain idempotent and pinned to major versions.
