---
type: decision
tags: [decision, fabric, direct-lake, cost-optimization]
date: 2026-04-14
project: "Interstellar Architecture Review & Cost Optimization"
status: accepted
---

# Decision: Interstellar — Direct Lake + Unity Catalog Mirroring

## Context
Interstellar architecture review identified capacity overage/idle time and cost inefficiency using Import/DirectQuery modes against a Databricks-backed source.

## Options Considered
1. Keep Import/DirectQuery, tune capacity manually.
2. Move to Direct Lake with Unity Catalog mirroring into OneLake (zero-copy).

## Decision
Refactor to Direct Lake with Unity Catalog mirroring — avoids data duplication (zero-copy), reduces capacity consumption, and consolidates capacity usage.

## Trade-offs
- Requires validating Direct Lake evaluation criteria (see [[Direct Lake]]) — model size, OneLake residency, near-real-time need.
- Adds a dependency on Unity Catalog mirroring maturity (see known limitations in [[Aurora PoC Program]]).

## Owner Agent
[[Atlas]] (architecture) + [[Treasurer]] (capacity/cost impact)

## Related
- Project: [[Interstellar Architecture Review & Cost Optimization]]
- Topics: [[Direct Lake]], [[Databricks Strategy]], [[Data Efficiency & FinOps]]
