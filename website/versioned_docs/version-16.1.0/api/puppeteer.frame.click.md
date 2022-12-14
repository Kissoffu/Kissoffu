---
sidebar_label: Frame.click
---

# Frame.click() method

This method clicks the first element found that matches `selector`.

**Signature:**

```typescript
class Frame {
  click(
    selector: string,
    options?: {
      delay?: number;
      button?: MouseButton;
      clickCount?: number;
    }
  ): Promise<void>;
}
```

## Parameters

| Parameter | Type                                                                                         | Description                                                                                     |
| --------- | -------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| selector  | string                                                                                       | the selector to search for to click. If there are multiple elements, the first will be clicked. |
| options   | { delay?: number; button?: [MouseButton](./puppeteer.mousebutton.md); clickCount?: number; } | <i>(Optional)</i>                                                                               |

**Returns:**

Promise&lt;void&gt;

## Remarks

This method scrolls the element into view if needed, and then uses [Page.mouse](./puppeteer.page.mouse.md) to click in the center of the element. If there's no element matching `selector`, the method throws an error.

Bear in mind that if `click()` triggers a navigation event and there's a separate `page.waitForNavigation()` promise to be resolved, you may end up with a race condition that yields unexpected results. The correct pattern for click and wait for navigation is the following:

```javascript
const [response] = await Promise.all([
  page.waitForNavigation(waitOptions),
  frame.click(selector, clickOptions),
]);
```
