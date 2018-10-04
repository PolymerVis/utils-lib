# PolymerVis

[![Greenkeeper badge](https://badges.greenkeeper.io/PolymerVis/utils-lib.svg)](https://greenkeeper.io/)

PolymerVis is a suite of Polymer elements for visualizations.

## Install

```bash
bower install PolymerVis/utils-lib --save
```

## Quick start
Import the `polymer-vis.html` file to use any of the utility functions.

```html
<link rel="import" href="../bower_components/utils-lib/utils-lib.html">
```

Alternatively, you can also include it as a script instead.
```html
<script src="../bower_components/utils-lib/utils-lib.js"></script>
```

## API reference
  <a name="exp_module_loadScript--PolymerVis.loadScript"></a>

## PolymerVis.loadScript(src, onload, onerror, optAsync) ⇒ <code>HTMLScriptElement</code> ⏏
Convenience method for dynamically loading a script.

This method creates a new `<script>` element with the provided URL and
appends it to the document to start loading. In the onload callback, the
import property of the link element will contain the imported document
contents.

**Kind**: global method of [<code>PolymerVis.loadScript</code>](#exp_module_loadScript--PolymerVis.loadScript)  

| Param | Type | Description |
| --- | --- | --- |
| src | <code>string</code> | The url to the script to load. |
| onload | <code>function</code> | callback when script is loaded. |
| onerror | <code>function</code> | callback when error loading script. |
| optAsync | <code>boolean</code> | whether to execute the script asynchronously. |

  <a name="exp_module_loadStylesheet--PolymerVis.loadStylesheet"></a>

## PolymerVis.loadStylesheet(href, onload, onerror, optAsync) ⇒ <code>HTMLLinkElement</code> ⏏
Convenience method for dynamically loading a stylesheet.

This method creates a new `<link rel="stylesheet">` element with the
provided URL and appends it to the document to start loading. In the onload
callback, the import property of the link element will contain the
imported document contents.

**Kind**: global method of [<code>PolymerVis.loadStylesheet</code>](#exp_module_loadStylesheet--PolymerVis.loadStylesheet)  

| Param | Type | Description |
| --- | --- | --- |
| href | <code>string</code> | The url to the script to load. |
| onload | <code>function</code> | callback when script is loaded. |
| onerror | <code>function</code> | callback when error loading script. |
| optAsync | <code>boolean</code> | whether to execute the script asynchronously. |

  <a name="exp_module_insertCssIntoShadowRoot--PolymerVis.insertCssIntoShadowRoot"></a>

## PolymerVis.insertCssIntoShadowRoot(cssSrc, shadowRoot, onload, id) ⏏
Load an external CSS file, and insert a `style` element
into the shadowRoot.

**Kind**: global method of [<code>PolymerVis.insertCssIntoShadowRoot</code>](#exp_module_insertCssIntoShadowRoot--PolymerVis.insertCssIntoShadowRoot)  

| Param | Type | Description |
| --- | --- | --- |
| cssSrc | <code>String</code> | url to the css file |
| shadowRoot | <code>String</code> | Node to insert the `style` element |
| onload | <code>function</code> | callback when CSS is inserted |
| id | <code>String</code> | id for style element |

**Example**  
```js
PolymerVis.insertCssIntoShadowRoot('https://some.css', ele.shadowRoot, 'custom');
```
  <a name="exp_module_isInShadowRoot--PolymerVis.isInShadowRoot"></a>

## PolymerVis.isInShadowRoot(node) ⇒ <code>Node</code> ⏏
Check if the node is inside a [`shadowRoot`](https://developer.mozilla.org/en-US/docs/Web/API/shadowRoot) or not.
Return the `shadowRoot` otherwise return `false`.

**Kind**: global method of [<code>PolymerVis.isInShadowRoot</code>](#exp_module_isInShadowRoot--PolymerVis.isInShadowRoot)  

| Param | Type | Description |
| --- | --- | --- |
| node | <code>Node</code> | the node to check |

