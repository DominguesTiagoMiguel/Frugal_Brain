# Workflow — Dev / Test / Prod Knowledge Base

This vault is version-controlled with Git and published to:
https://github.com/DominguesTiagoMiguel/Frugal_Brain

## Branches
- **dev** — active working branch. New/edited notes land here first (drafts, in-progress research).
- **test** — staging branch. Content promoted from `dev` once it looks ready, for a final review pass.
- **main** (prod) — the published, trusted knowledge base. Only reviewed/approved content lives here.

## Promotion process (manual approval)
1. Work happens on `dev` (adding/editing notes on any topic).
2. When a note (or set of notes) is ready, a diff is shown between `dev` and `test`.
3. You approve → changes are merged into `test`.
4. After a final check on `test`, you approve → changes are merged into `main` and pushed to GitHub.

No promotion happens automatically — every step from dev → test → prod requires your explicit approval.

## Folder structure
- `00 - Inbox` — quick captures, unsorted notes
- `01 - Topics` — organized knowledge notes, one per topic
- `02 - MOCs` — Maps of Content (index/hub notes), e.g. this file and `Home.md`
- `03 - Templates` — note templates (e.g. `Topic Template.md`)

## Notes on `.obsidian/`
The `.obsidian/` folder (plugin settings, local API keys, workspace state) is intentionally
excluded from git via `.gitignore`. It contains machine-local secrets (e.g. Local REST API
plugin keys) that must never be committed to a public repository.
