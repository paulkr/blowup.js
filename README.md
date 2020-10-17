blowup.js
===========

A jQuery plugin for customizable image magnification.

[Check out a demo!](http://paulkr.github.io/blowup.js)

<img src="https://raw.githubusercontent.com/paulkr/blowup.js/gh-pages/blowup.png" width="500" />

Usage
-----

You can install blowup through npm:

```bash
$ npm install blowup
```

or through bower:

```bash
$ bower install blowup
```

Alternatively, download the package and reference the `blowup.js` file in your HTML file. 
Ensure you have included the latest stable jQuery version before including `blowup.js`.

```html
<script src="//ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>
<script type="text/javascript" src="lib/blowup.js"></script>
```

Then, apply the blowup effect to your image.

```javascript
$(document).ready(function () {
    $("img").blowup();
})
```

Configuration Parameters
------------------------

Listed are the customization options that `blowup.js` allows. 

<table style="width:100%">
    <tr>
        <th>Parameter</th>
        <th>Purpose</th>
        <th>Default</th>
    <tr>
        <td>round</td>
        <td>If you want the magnification lens to be round. <br />Setting this to false will give you a square lens.</td>
        <td>true</td>
    </tr>
    <tr>
        <td>width</td>
        <td>Lens Width in pixels.</td>
        <td>200</td>
    </tr>
    <tr>
        <td>height</td>
        <td>Lens height in pixels.</td>
        <td>200</td>
    </tr>
    <tr>
        <td>background</td>
        <td>Color for background (will be visible on image edges).</td>
        <td>"#FFF"</td>
    </tr>
    <tr>
        <td>shadow</td>
        <td>CSS style for lens shadow.</td>
        <td>"0 8px 17px 0 rgba(0, 0, 0, 0.2)"</td>
    </tr>
    <tr>
        <td>border</td>
        <td>CSS style for lens border.</td>
        <td>"6px solid #FFF"</td>
    </tr>
    <tr>
        <td>cursor</td>
        <td>Set to false if you do not want the crosshair cursor visible.</td>
        <td>true</td>
    </tr>
    <tr>
        <td>zIndex</td>
        <td>z-index value of the lens.</td>
        <td>999999</td>
    </tr>
    <tr>
        <td>scale</td>
        <td>Scale factor for zoom.</td>
        <td>1</td>
    </tr>
    <tr>
        <td>customClasses</td>
        <td>Additional CSS classes to add to the magnification (separated by spaces).</td>
        <td>""</td>
    </tr>
</table>

#### Example

```javascript
$("img").blowup({
    "background" : "#F39C12",
    "width" : 250,
    "height" : 250,
    "customClasses" : "class1 class2"
})
```
