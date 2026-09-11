---
tags: [moc, cache]
status: active
created: 2026-09-11
---

# Knowledge Cache — Index

This is the living cache of everything captured from interactions with the user: meetings, brainstorms, discussions, and ad-hoc context. It is how the agents ([[Atlas]], [[Curator]], [[Treasurer]], [[Maestro]]) build memory over time, distinct from the curated, stable knowledge in [[03 - Topics]].

**Folders:**
- `Sessions/` — one note per working session/interaction (use [[Session Log Template]]).
- `Decisions/` — ADR-style decision records (use [[Decision Record Template]]).
- `Brainstorms/` — raw brainstorm captures (use [[Brainstorm Template]]).

## Browse by recency (all cache items)
```dataview
TABLE type, date, project, urgency, status
FROM "04 - Knowledge Cache"
WHERE type
SORT date DESC
```

## Browse by project
```dataview
TABLE type, date, urgency, status
FROM "04 - Knowledge Cache"
WHERE type AND project != ""
GROUP BY project
SORT date DESC
```

## Browse by urgency (Eisenhower-style triage)
```dataview
TABLE type, date, project, status
FROM "04 - Knowledge Cache"
WHERE urgency = "high"
SORT date DESC
```

## Browse by sprint
```dataview
TABLE type, date, project, status
FROM "04 - Knowledge Cache"
WHERE sprint != ""
GROUP BY sprint
SORT date DESC
```

## Open items (not yet processed into Topics/Decisions)
```dataview
TABLE type, date, project
FROM "04 - Knowledge Cache"
WHERE status = "captured" OR status = "raw"
SORT date DESC
```

## Related
- [[03 - Topics]] (stable, curated knowledge — promote cache items here once mature)
- [[05 - Projects]]
- [[Agents Index]]
