---
tags: [template]
---
---
type: project
tags: [project]
status: active
start_date: <% tp.date.now("YYYY-MM-DD") %>
sprint: ""
urgency: medium
---

# <% tp.file.title %>

## One-line objective
_

## Scope
-

## Knowledge Cache links
_(sessions, decisions, brainstorms tied to this project — Dataview query below will auto-populate once `project` frontmatter matches this note's title)_

```dataview
TABLE date, type, status
FROM "04 - Knowledge Cache"
WHERE contains(project, this.file.name)
SORT date DESC
```

## Related Topics
- [[]]

## Related Agents
- [[]]
