---
tags: [topic, fabric, platform-strategy, legacy]
status: active
created: 2026-09-11
source: "Knowledge_Base_Fabric_Data_Architecture_Agent.md"
---

# Microsoft Fabric Strategy

## Strategic Positioning
Microsoft Fabric is the primary analytics platform integrating: Data Engineering, Data Science, Data Warehousing, Real-Time Analytics, Power BI.

## Governance Model — Workspace Classification
1. **Critical Interactive Workloads** — executive reporting, operational dashboards, target rendering <5 seconds.
2. **Standard Interactive Workloads** — department reporting, self-service analytics.
3. **Background Workloads** — ETL, batch processing, data refresh.

## Capacity Management Principles
- Assign workspaces according to workload profile.
- Prefer automated placement.
- Monitor actual versus declared usage.
- Separate critical and background workloads when justified.

## Migration Principles — Power BI to Fabric
- Assess workspace readiness.
- Validate semantic models.
- Review refresh strategy.
- Evaluate Direct Lake opportunities.
- Verify ownership and support model.

## Related
- [[Semantic Models]]
- [[Direct Lake]]
- [[Databricks Strategy]]
- [[Workload & Platform Strategy]]
- [[Atlas]]
