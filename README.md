cesium-drawhelper
================

This project builds off the work done by [leforthomas](https://github.com/leforthomas/cesium-drawhelper), [williamscs](https://github.com/williamscs/cesium-drawhelper) and [smills](https://github.com/smills2929/cesium-drawhelper). We created an ACEs fork to add a package.json file (so we can can manage cesium-drawhelper through NPM specifically), and to keep the plugin working with versions of cesium as it is updated.

Cesium version: Tested against Cesium v1.22

License: Apache 2.0. Free for commercial and non-commercial use. See LICENSE.md.

Usage:

Import the DrawHelper.js, DrawHelper.css and /img/ image files into your directory. Add script and css files to your page.

Instantiate a drawHelper passing it the CesiumWidget.

You can:
- use the self contained drawing widget by calling the drawHelper.addToolbar(container, options). This will add a drawing toolbar to the specified container. Options are for personalising the display of the shapes. The toolbar issues one creation event per shape created. You can listen to those events by calling the addListener method.
- use the startDrawXXX methods of DrawHelper to create shapes interactively
- enable editing of your primitives (at the moment Billboard, Polygon, ExtentPrimitive, DrawHelper.CirclePrimitive, DrawHelper.EllipsePrimitive and DrawHelper.PolylinePrimitive) by calling their setEditable method.

The toolbar can be customised at creation by passing an option object.

Check the index.html example to get started.

Check the website http://pad.geocento.com/DrawHelper/ for a live example of the older https://github.com/leforthomas/cesium-drawhelper version.

Future versions will include shape dragging, scaling and rotation and support for hierarchical polygon editing.
