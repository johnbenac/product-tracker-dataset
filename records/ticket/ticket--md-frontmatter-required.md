---
id: ticket:md-frontmatter-required
datasetId: dataset:product-tracker
typeId: ticket
createdAt: 2025-12-10T16:45:00Z
updatedAt: 2025-12-27T08:00:00Z
fields:
  title: "Require YAML front matter on all records"
  status: done
  priority: high
  project: project:core-app
  assignee: person:johnny
  tags:
    - tag:import
---
Description:
Importer must fail with a file-specific error if YAML front matter is missing or invalid.
