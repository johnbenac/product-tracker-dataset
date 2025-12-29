---
id: type:decision
datasetId: dataset:product-tracker
typeId: sys:type
createdAt: 2025-12-01T00:00:00Z
updatedAt: 2025-12-01T00:00:00Z
fields:
  recordTypeId: decision
  displayName: Decision
  pluralName: Decisions
  icon: file-text
  bodyField: content

  fieldDefs:
    title:
      kind: string
      required: true
      ui:
        label: Title

    status:
      kind: enum
      required: true
      options: [proposed, accepted, rejected, superseded]
      default: proposed
      ui:
        label: Status

    date:
      kind: date
      ui:
        label: Date

    project:
      kind: ref
      ui:
        label: Project
        refTypeHints: [project]

    relatedTickets:
      kind: ref[]
      ui:
        label: Related tickets
        refTypeHints: [ticket]
---
