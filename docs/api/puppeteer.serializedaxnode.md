---
sidebar_label: SerializedAXNode
---

# SerializedAXNode interface

Represents a Node and the properties of it that are relevant to Accessibility.

**Signature:**

```typescript
export interface SerializedAXNode
```

## Properties

| Property                                                            | Modifiers | Type                                                    | Description                                                                                                                                                      |
| ------------------------------------------------------------------- | --------- | ------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [autocomplete?](./puppeteer.serializedaxnode.autocomplete.md)       |           | string                                                  | <i>(Optional)</i>                                                                                                                                                |
| [checked?](./puppeteer.serializedaxnode.checked.md)                 |           | boolean \| 'mixed'                                      | <i>(Optional)</i> Whether the checkbox is checked, or in a [mixed state](https://www.w3.org/TR/wai-aria-practices/examples/checkbox/checkbox-2/checkbox-2.html). |
| [children?](./puppeteer.serializedaxnode.children.md)               |           | [SerializedAXNode](./puppeteer.serializedaxnode.md)\[\] | <i>(Optional)</i> Children of this node, if there are any.                                                                                                       |
| [description?](./puppeteer.serializedaxnode.description.md)         |           | string                                                  | <i>(Optional)</i> An additional human readable description of the node.                                                                                          |
| [disabled?](./puppeteer.serializedaxnode.disabled.md)               |           | boolean                                                 | <i>(Optional)</i>                                                                                                                                                |
| [expanded?](./puppeteer.serializedaxnode.expanded.md)               |           | boolean                                                 | <i>(Optional)</i>                                                                                                                                                |
| [focused?](./puppeteer.serializedaxnode.focused.md)                 |           | boolean                                                 | <i>(Optional)</i>                                                                                                                                                |
| [haspopup?](./puppeteer.serializedaxnode.haspopup.md)               |           | string                                                  | <i>(Optional)</i>                                                                                                                                                |
| [invalid?](./puppeteer.serializedaxnode.invalid.md)                 |           | string                                                  | <i>(Optional)</i> Whether and in what way this node's value is invalid.                                                                                          |
| [keyshortcuts?](./puppeteer.serializedaxnode.keyshortcuts.md)       |           | string                                                  | <i>(Optional)</i> Any keyboard shortcuts associated with this node.                                                                                              |
| [level?](./puppeteer.serializedaxnode.level.md)                     |           | number                                                  | <i>(Optional)</i> The level of a heading.                                                                                                                        |
| [modal?](./puppeteer.serializedaxnode.modal.md)                     |           | boolean                                                 | <i>(Optional)</i>                                                                                                                                                |
| [multiline?](./puppeteer.serializedaxnode.multiline.md)             |           | boolean                                                 | <i>(Optional)</i>                                                                                                                                                |
| [multiselectable?](./puppeteer.serializedaxnode.multiselectable.md) |           | boolean                                                 | <i>(Optional)</i> Whether more than one child can be selected.                                                                                                   |
| [name?](./puppeteer.serializedaxnode.name.md)                       |           | string                                                  | <i>(Optional)</i> A human readable name for the node.                                                                                                            |
| [orientation?](./puppeteer.serializedaxnode.orientation.md)         |           | string                                                  | <i>(Optional)</i>                                                                                                                                                |
| [pressed?](./puppeteer.serializedaxnode.pressed.md)                 |           | boolean \| 'mixed'                                      | <i>(Optional)</i> Whether the node is checked or in a mixed state.                                                                                               |
| [readonly?](./puppeteer.serializedaxnode.readonly.md)               |           | boolean                                                 | <i>(Optional)</i>                                                                                                                                                |
| [required?](./puppeteer.serializedaxnode.required.md)               |           | boolean                                                 | <i>(Optional)</i>                                                                                                                                                |
| [role](./puppeteer.serializedaxnode.role.md)                        |           | string                                                  | The [role](https://www.w3.org/TR/wai-aria/#usage_intro) of the node.                                                                                             |
| [roledescription?](./puppeteer.serializedaxnode.roledescription.md) |           | string                                                  | <i>(Optional)</i> A human readable alternative to the role.                                                                                                      |
| [selected?](./puppeteer.serializedaxnode.selected.md)               |           | boolean                                                 | <i>(Optional)</i>                                                                                                                                                |
| [value?](./puppeteer.serializedaxnode.value.md)                     |           | string \| number                                        | <i>(Optional)</i> The current value of the node.                                                                                                                 |
| [valuemax?](./puppeteer.serializedaxnode.valuemax.md)               |           | number                                                  | <i>(Optional)</i>                                                                                                                                                |
| [valuemin?](./puppeteer.serializedaxnode.valuemin.md)               |           | number                                                  | <i>(Optional)</i>                                                                                                                                                |
| [valuetext?](./puppeteer.serializedaxnode.valuetext.md)             |           | string                                                  | <i>(Optional)</i> A description of the current value.                                                                                                            |
