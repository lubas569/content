---
title: 'Window: vrdisplaypointerunrestricted event'
slug: Web/API/Window/vrdisplaypointerunrestricted_event
page-type: web-api-event
tags:
  - Reference
  - WebVR
  - Window
  - Event
  - Deprecated
  - vrdisplaypointerunrestricted
browser-compat: api.Window.vrdisplaypointerunrestricted_event
---
{{APIRef("Window")}}{{Deprecated_Header}}

The **`vrdisplaypointerunrestricted`** event of the [WebVR API](/en-US/docs/Web/API/WebVR_API) is fired when the VR display's pointer input is no longer restricted to consumption via a [pointerlocked element](/en-US/docs/Web/API/Pointer_Lock_API).

> **Note:** This event was part of the old [WebVR API](https://immersive-web.github.io/webvr/spec/1.1/). It has been superseded by the [WebXR Device API](https://immersive-web.github.io/webxr/).

This event is not cancelable and does not bubble.

## Syntax

Use the event name in methods like {{domxref("EventTarget.addEventListener", "addEventListener()")}}, or set an event handler property.

```js
addEventListener('vrdisplaypointerunrestricted', (event) => { });

onvrdisplaypointerunrestricted = (event) => { };
```

## Event type

An {{domxref("VRDisplayEvent")}}. Inherits from {{domxref("Event")}}.

{{InheritanceDiagram("VRDisplayEvent")}}

## Event properties

_`VRDisplayEvent` also inherits properties from its parent object, {{domxref("Event")}}._

- {{domxref("VRDisplayEvent.display")}} {{deprecated_inline}} {{readonlyInline}}
  - : The {{domxref("VRDisplay")}} associated with this event.
- {{domxref("VRDisplayEvent.reason")}} {{deprecated_inline}} {{readonlyInline}}
  - : A human-readable reason why the event was fired.

## Examples

You can use the `vrdisplaypointerunrestricted` event in an [`addEventListener`](/en-US/docs/Web/API/EventTarget/addEventListener) method:

```js
window.addEventListener('vrdisplaypointerunrestricted', () => {
  // Run code to handle freeing app from pointer lock
});
```

Or use the `onvrdisplaypointerunrestricted` event handler property:

```js
window.onvrdisplaypointerunrestricted = () => {
  // Run code to handle freeing app from pointer lock
};
```

## Specifications

This event was part of the old [WebVR API](https://immersive-web.github.io/webvr/spec/1.1/) that has been superseded by the [WebXR Device API](https://immersive-web.github.io/webxr/). It is no longer on track to becoming a standard.

Until all browsers have implemented the new [WebXR Device API](https://immersive-web.github.io/webxr/), it is recommended to rely on frameworks, like [A-Frame](https://aframe.io/), [Babylon.js](https://www.babylonjs.com/), or [Three.js](https://threejs.org/), or a [polyfill](https://github.com/immersive-web/webxr-polyfill), to develop WebXR applications that will work across all browsers [\[1\]](https://developer.oculus.com/documentation/web/port-vr-xr/).

## Browser compatibility

{{Compat}}

## See also

- [WebVR API homepage](/en-US/docs/Web/API/WebVR_API)
- <https://mixedreality.mozilla.org/> — demos, downloads, and other resources from the Mozilla VR team.
