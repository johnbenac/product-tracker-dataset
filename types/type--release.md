---
id: type:release
datasetId: dataset:product-tracker
typeId: sys:type
createdAt: 2025-12-30T00:00:00Z
updatedAt: 2025-12-30T00:00:00Z
fields:
  recordTypeId: release
  displayName: Release
  pluralName: Releases
  icon: flag
  bodyField: summary
  composition:
    project:
      recordTypeId: project
      min: 1
      max: 1
    ticket:
      recordTypeId: ticket
      min: 1
  fieldDefs:
    name:
      kind: string
      required: true
    projectRefs:
      kind: ref[]
      ui:
        label: Projects
        refTypeHints: [project]
    ticketRefs:
      kind: ref[]
      ui:
        label: Tickets
        refTypeHints: [ticket]
    summary:
      kind: string
---
