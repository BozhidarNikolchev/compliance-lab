

<!--
Title: Day 8 – NIST CSF Portfolio Pack (EN)
Author: Bozhidar Nikolchev  
Program: 30-Day Compliance – Day 8 (NIST CSF)
Date: 2026-03-03
-->


# Day 8 – NIST Cybersecurity Framework (CSF) 2.0

This folder is optimized for **VS Code** and **GitHub**. It contains:

- **Docs** (`/docs`) – deep-dive guides: CSF Core, Profiles & Tiers, Implementation Plan, Gap Analysis, SCRM, References.
- **Templates** (`/templates`) – ready-to-use YAML/CSV templates: **Current/Target Profiles**, **POA&M**, **Risk Register**, **Asset Inventory**, **Control Owners**, **KPIs** and policy/runbook stubs.
- **Mappings** (`/mappings`) – CSF ⇄ ISO 27001 ⇄ GDPR examples.
- **Diagrams** (`/diagrams`) – Mermaid diagrams rendered natively by GitHub.
- **Automation & Quality** – `.vscode/`, `.config/markdownlint.json`, `.editorconfig`, and a GitHub Action for Markdown linting.

> CSF 2.0 includes **six functions** (adding **Govern**) and uses **Organizational Profiles** and **CSF Tiers** to express outcomes and maturity.

## Quick Start
1. Open in **VS Code** → install recommended extensions.
2. Fill out `/templates/profile_current.yaml` and `/templates/profile_target.yaml`.
3. Compare Profiles using `/docs/04_Gap_Analysis_Guide.md` and populate `/templates/poam.csv`.
4. Commit changes and push to GitHub.
