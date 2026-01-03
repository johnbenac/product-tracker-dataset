---
typeId: ticket
fields:
  displayName: Ticket
  pluralName: Tickets
  icon: check-square
  bodyField: description

  fieldDefs:
    title:
      kind: string
      required: true
      ui:
        label: Title
        placeholder: "Short, specific summary…"

    status:
      kind: enum
      required: true
      options: [backlog, in_progress, blocked, done]
      default: backlog
      ui:
        label: Status

    priority:
      kind: enum
      options: [low, medium, high, urgent]
      default: medium
      ui:
        label: Priority

    project:
      kind: ref
      required: true
      ui:
        label: Project
        refTypeHints: [project]

    assignee:
      kind: ref
      ui:
        label: Assignee
        refTypeHints: [person]

    tags:
      kind: ref[]
      ui:
        label: Tags
        widget: chips
        refTypeHints: [tag]

    dueDate:
      kind: date
      ui:
        label: Due date

    estimatePoints:
      kind: number
      constraints:
        min: 0
        max: 100
      ui:
        label: Estimate (points)

    blockedBy:
      kind: ref[]
      ui:
        label: Blocked by
        refTypeHints: [ticket]

    links:
      kind: ref[]
      ui:
        label: Links
        help: "Free-form graph edges; can point to any record type."
---
