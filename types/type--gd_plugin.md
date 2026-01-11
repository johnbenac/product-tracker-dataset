---
typeId: gd_plugin
fields:
  displayName: GD Plugin
  pluralName: GD Plugins
  icon: plug
  bodyField: notes

  fieldDefs:
    pluginId:
      kind: string
      required: true
      ui:
        label: Plugin ID

    enabled:
      kind: boolean
      required: false
      default: true
      ui:
        label: Enabled

    entry:
      kind: string
      required: true
      ui:
        label: Entry module (block CID)
        help: 'CID wiki-link like [[bafk...]]'

    notes:
      kind: string
      required: false
      ui:
        label: Notes
---
