# Static helper class for Greensock properties
Static JavaScript helper class that simply accepts either a Javascript or jQuery obj (‘element’ or $(“element”)) and returns the Greensock property for that object.

- **Author**: Chris Gannon
- **Source**: http://blog.gannon.tv/2013/01/11/greensock-properties-helper-class-for-javascript-and-jquery/

### Usage
This adds the Greensock _gsTransform object to your element - it doesn't need to have any visual effect at all
```TweenLite.set(myElement, {css:{x:0}});```
Then, when you want to, say, retrieve the current rotationY or scaleX of an element you can simply write:

```var myElementRotationY = GreenProp.rotationY(myElement);``` - passing in a JavaScript element, or

```var myElementScaleX = GreenProp.scaleX($("cube"));``` passing in a jQuery element

The properties it can return are as follows:
- rotationX
- rotationY
- rotationZ (you can pass in either rotationZ or just rotation)
- scaleX
- scaleY
- scaleZ
- x
- y
- z
- perspective
- skewX
- skewY
- zOrigin