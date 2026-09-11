---
type: project
tags: [project, fabric, bigquery, aurora, active, legacy]
status: active
start_date: ""
sprint: ""
urgency: medium
---

# Aurora PoC Program

## One-line objective
Client Solutions PoC integrating Microsoft Fabric with GCP/BigQuery and Google Storage, including Salesforce ingestion paths.

## Scope
- Fabric ↔ BigQuery success metrics and integration patterns.
- Salesforce → Fabric ingestion (Delta Sharing, mirroring, REST connector options).
- Databricks Unity Catalog mirroring into Fabric — limitations and private endpoint/VNet requirements identified.

## Key open threads
- Unity Catalog mirroring limitations (see [[Databricks Strategy]]).
- Private endpoint requirements for Databricks mirroring into Fabric (security/network dependency).

## Related Topics
- [[Microsoft Fabric Strategy]]
- [[Databricks Strategy]]
- [[Direct Lake]]

## Related Agents
- [[Atlas]] (cross-platform architecture: Fabric + BigQuery + Databricks)
- [[Treasurer]] (cost of cross-cloud data movement/egress)

## Source
Full history lives in the operational vault: `Obsidian/00 - Inbox/*Aurora*`, `Obsidian/00 - Inbox/Delta Sharing Salesforce.md`, `Obsidian/00 - Inbox/Fabric Items Mirrored Unity Catalog *.md`.
