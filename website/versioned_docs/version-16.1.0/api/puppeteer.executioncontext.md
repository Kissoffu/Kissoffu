---
sidebar_label: ExecutionContext
---

# ExecutionContext class

This class represents a context for JavaScript execution. A \[Page\] might have many execution contexts: - each [frame](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe) has "default" execution context that is always created after frame is attached to DOM. This context is returned by the [Frame.executionContext()](./puppeteer.frame.executioncontext.md) method. - [Extension](https://developer.chrome.com/extensions)'s content scripts create additional execution contexts.

Besides pages, execution contexts can be found in [workers](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API).

**Signature:**

```typescript
export declare class ExecutionContext
```

## Remarks

The constructor for this class is marked as internal. Third-party code should not call the constructor directly or create subclasses that extend the `ExecutionContext` class.

## Methods

| Method                                                                               | Modifiers | Description                                                                                  |
| ------------------------------------------------------------------------------------ | --------- | -------------------------------------------------------------------------------------------- |
| [evaluate(pageFunction, args)](./puppeteer.executioncontext.evaluate.md)             |           |                                                                                              |
| [evaluateHandle(pageFunction, args)](./puppeteer.executioncontext.evaluatehandle.md) |           |                                                                                              |
| [frame()](./puppeteer.executioncontext.frame.md)                                     |           |                                                                                              |
| [queryObjects(prototypeHandle)](./puppeteer.executioncontext.queryobjects.md)        |           | This method iterates the JavaScript heap and finds all the objects with the given prototype. |
