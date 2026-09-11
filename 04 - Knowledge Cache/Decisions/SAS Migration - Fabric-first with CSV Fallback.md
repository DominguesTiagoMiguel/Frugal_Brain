---
type: decision
tags: [decision, fabric, sas-migration]
date: 2026-04-30
project: "SAS Migration Phase 2"
status: accepted
---

# Decision: SAS Migration - Fabric-first with CSV Fallback

## Context
During development/handover of the SAS → Fabric Phase 2 migration, a standard needed to be set for process outputs.

## Options Considered
1. Keep CSV as the default output format (matches legacy SAS behavior).
2. Fabric-native output (Delta Tables) as default, CSV only where a downstream consumer strictly requires it.

## Decision
Fabric-first: outputs should be Delta Tables. CSV is a fallback only, not the default.

## Trade-offs
- Slightly more migration effort per process to validate Delta Table consumers.
- Long-term reduction in file-based sprawl and duplication; consistent with [[Reference Architecture]] and [[Data Engineering Standards]].

## Owner Agent
[[Atlas]]

## Related
- Project: [[SAS Migration Phase 2]]
- Topics: [[Microsoft Fabric Strategy]]
