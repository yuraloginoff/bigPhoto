# bigPhoto

bigPhoto is a jQuery plugin to proportionally stretch images to their ancestor's width.
The width can be set in percents or in pixels. In case of pixels images become responsive.

You can see it in action on this [demo page](http://yuraloginoff.com/bigphoto/)

## How to install

1. Add CSS to the `<head>`:
```
	<link rel="stylesheet" href="css/jquery.bigphoto.css">
```

2. Add JavaScript before the `</body>`:
```
	<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.10.1/jquery.min.js"></script>
	<script src="js/jquery.bigphoto.js"></script>
	<script>
		$("img.bigphoto-img").bigPhoto();
	</script>
```

## Markup

The following type of markup structure is needed to make the plugin work:

	<div class="bigphoto-wrap">
		<img src="img/01.jpg" class="bigphoto-img">
	</div>

## JavaScript
Running this script will apply the bigPhoto plugin to images with class "bigphoto-img".
```javascript
$("img.bigphoto-img").bigPhoto();
```

You can pass an object to bigPhoto function to redefine default settings, f.i.:
```javascript
$("#slider").sliderify({
	imageWrapperWidth : "100%"
});
```

Here is a list of all settings that you can redefine.

Setting | Default | Description
--- | --- | ---
imageWrapperWidth | "100%" | With this setting you can set the parent width. All images will stretch to it. If you set width in pixels, f.i. "600px", images will be responsive.
wrapClass | "bigphoto-wrap" | Images parent class name. Don't foreget also to change it in css file!
onWindowResize | true | Set to false if you don't wang images to be stretched on window resize.


## Credits
Initially written by [Yura Loginov](http://yuraloginoff.com).

If you have any questions about this plugin please contact me on twitter - [@yuraloginoff](https://twitter.com/yuraloginoff)

## Legal

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <http://unlicense.org/>
