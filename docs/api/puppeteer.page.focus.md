---
sidebar_label: Page.focus
---

# Page.focus() method

This method fetches an element with `selector` and focuses it. If there's no element matching `selector`, the method throws an error.

**Signature:**

```typescript
class Page {
  focus(selector: string): Promise<void>;
}
```

## Parameters

| Parameter | Type   | Description                                                                                                                                                                             |
| --------- | ------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| selector  | string | A [selector](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors) of an element to focus. If there are multiple elements satisfying the selector, the first will be focused. |

**Returns:**

Promise&lt;void&gt;

Promise which resolves when the element matching selector is successfully focused. The promise will be rejected if there is no element matching selector.

## Remarks

Shortcut for [page.mainFrame().focus(selector)](./puppeteer.frame.focus.md).
