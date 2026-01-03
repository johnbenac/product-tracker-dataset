---
typeId: decision
recordId: md-as-canonical
fields:
  title: "Markdown repositories are canonical"
  status: accepted
  date: 2025-12-12
  project: "[[project:core-app]]"
  relatedTickets:
    - "[[ticket:wiki-links]]"
---
## Context
We need import/export round-trips that preserve human intent and diffs.

## Decision
All records are Markdown files with YAML front matter.
GitHub repositories are the primary interchange format.

## Consequences
- Relationships may be explicit fields or `[[id]]` wiki-links.
