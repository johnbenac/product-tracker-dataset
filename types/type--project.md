---
typeId: project
fields:
  displayName: Project
  pluralName: Projects
  icon: folder
  bodyField: overview

  fieldDefs:
    name:
      kind: string
      required: true
      constraints:
        minLength: 2
      ui:
        label: Name

    status:
      kind: enum
      options: [planned, active, paused, done]
      default: active
      ui:
        label: Status

    owner:
      kind: ref
      ui:
        label: Owner
        refTypeHints: [person]

    budget:
      kind: money
      ui:
        label: Budget
        currency: USD

    tags:
      kind: ref[]
      ui:
        label: Tags
        refTypeHints: [tag]
---
