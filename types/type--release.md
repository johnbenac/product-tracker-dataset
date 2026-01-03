---
typeId: release
fields:
  displayName: Release
  pluralName: Releases
  icon: flag
  bodyField: summary

  composition:
    project:
      typeId: project
      required: true
    ticket:
      typeId: ticket
      required: true

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
