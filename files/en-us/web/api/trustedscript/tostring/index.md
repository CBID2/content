---
title: "TrustedScript: toString() method"
short-title: toString()
slug: Web/API/TrustedScript/toString
page-type: web-api-instance-method
browser-compat: api.TrustedScript.toString
---

{{APIRef("Trusted Types API")}}{{AvailableInWorkers}}

The **`toString()`** method of the {{domxref("TrustedScript")}} interface returns a string which may be safely inserted into an [injection sink](/en-US/docs/Web/API/Trusted_Types_API#concepts_and_usage).

## Syntax

```js-nolint
toString()
```

### Parameters

None.

### Return value

A string containing the sanitized script.

## Examples

The constant `sanitized` is an object created via a Trusted Types policy. The `toString()` method returns a string to safely execute as a script.

```js
const sanitized = scriptPolicy.createScript("eval('2 + 2')");
console.log(sanitized.toString());
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
