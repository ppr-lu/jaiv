# JustAnotherImageViewer

An Image Viever done in JavaScript.

### How to use it

Does not depend of jQuery (supposedly).
This library has fabric.js as its dependency. Only version 1.4.0 has been tested, so it may not work for other versions.
Version 1.4.0 can be found in dist/ folder:

```javascript
<script src="dist/fabric.min.js"></script>
```
or

```javascript
<script src="http://cdnjs.cloudflare.com/ajax/libs/fabric.js/1.4.0/fabric.min.js"></script>
```

To initialize it:
```javascript
var config = {
            //Element which content is overriden with the image viewer
            element: document.getElementById("replace"),
            //Rows in the image viewer
            rows: 2,
            //columns in the image viewer
            columns: 2,
            //Array with the raw data of the images. Can also be a single string.
            //Example of this can be found in example/rawImageData.js
            imageData: aRawImageData,
            //If true => resize image to fit canvas
            //false => resize canvas to fit original image size
            adaptImageToCanvas: true,
            // width of the canvas in case adaptImageToCanvas is true
            width: 600,
            // height of the canvas in case adaptImageToCanvas is true
            height: 338
        };
jaiv.initImageViewer(config);
```
Check example/lu.html for an example.

