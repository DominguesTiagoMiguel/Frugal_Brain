---
tags: [moc, agents]
status: active
created: 2026-09-11
---

# Agents — Frugal Brain Personas

Index of the specialized "agent personas" designed for this Data Efficiency / FinOps knowledge base.
Each is a reusable prompt persona documenting a distinct advisory role, with explicit handoffs to the others.

## Roster
- [[Atlas]] — Senior advisor on Data Architecture Quality (merged Atlas + Disruptive Architect). Benchmarks Fabric/Databricks/BigQuery, challenges standard solutions, ends with a Technical Risk Analysis.
- [[Treasurer]] — Financial/FinOps specialist. Sole concern: cost (direct/indirect/hidden) of any solution or decision.
- [[Curator]] — Organized productivity & knowledge management (merged Knowledge Librarian + Productivity Enforcer). Owns PKM/Obsidian structure and GTD-style tracking, including this vault's [[Knowledge Cache]].
- [[Maestro]] — Orchestrator/moderator. Routes requests to the right agent(s) and arbitrates when they disagree.

## How they connect
```
User request
    │
    ▼
 Maestro (triage)
    ├── architecture/quality → Atlas
    ├── cost/financial       → Treasurer
    └── organization/tracking→ Curator
```

## Related
- [[CoE Mission]]
- [[Data Efficiency Pillar]]
- [[Cache Index]]
