## Canvas element
A canvas looks like the img element, with the only difference being that it doesn't have the src and alt attributes, only width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.  

Providing fallback content is very straightforward: just insert the alternate content inside the canvas element. Browsers that don't support canvas will ignore the container and render the fallback content inside it. Browsers that do support canvas will ignore the content inside the container, and just render the canvas normally. Canvas also needs a closing tag.  

## Drawing in canvas
You can only draw rectangles and lines in canvas... That's it.  

_fillRect(x, y, width, height)_ Draws a filled rectangle.  
_strokeRect(x, y, width, height)_ Draws a rectangular outline.  
_clearRect(x, y, width, height)_ Clears the specified rectangular area, making it fully transparent.  

Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.

_beginPath()_ Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.  
_closePath()_ Adds a straight line to the path, going to the start of the current sub-path.  
_stroke()_ Draws the shape by stroking its outline.  
_fill()_ Draws a solid shape by filling the path's content area.  

The first step to create a path is to call the beginPath(). Internally, paths are stored as a list of sub-paths (lines, arcs, etc) which together form a shape. Every time this method is called, the list is reset and we can start drawing new shapes.  

_quadraticCurveTo(cp1x, cp1y, x, y)_ Draws a quadratic Bézier curve from the current pen position to the end point specified by x and y, using the control point specified by cp1x and cp1y.  
_bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)_ Draws a cubic Bézier curve from the current pen position to the end point specified by x and y, using the control points specified by (cp1x, cp1y) and (cp2x, cp2y).  

The difference between these can best be described using the image on the right. A quadratic Bézier curve has a start and an end point (blue dots) and just one control point (indicated by the red dot) while a cubic Bézier curve uses two control points.  

The x and y parameters in both of these methods are the coordinates of the end point. cp1x and cp1y are the coordinates of the first control point, and cp2x and cp2y are the coordinates of the second control point.  

Using quadratic and cubic Bézier curves can be quite challenging, because unlike vector drawing software like Adobe Illustrator, we don't have direct visual feedback as to what we're doing. This makes it pretty hard to draw complex shapes. In the following example, we'll be drawing some simple organic shapes, but if you have the time and, most of all, the patience, much more complex shapes can be created.  

## Colors

_fillStyle = color_  
Sets the style used when filling shapes.  
_strokeStyle = color_  
Sets the style for shapes' outlines.  
_globalAlpha = transparencyValue_  
Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.  

## Line styles
_lineWidth = value_ Sets the width of lines drawn in the future.  
_lineCap = type_ Sets the appearance of the ends of lines.  
_lineJoin = type_ Sets the appearance of the "corners" where lines meet.  
_miterLimit = value_ Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.  
_getLineDash()_ Returns the current line dash pattern array containing an even number of non-negative numbers.  
_setLineDash(segments)_ Sets the current line dash pattern.  
_lineDashOffset = value_ Specifies where to start a dash array on a line.  

_createLinearGradient(x1, y1, x2, y2)_  
Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).  
_createRadialGradient(x1, y1, r1, x2, y2, r2)_  
Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.  
_gradient.addColorStop(position, color)_  
Creates a new color stop on the gradient object. The position is a number between 0.0 and 1.0 and defines the relative position of the color in the gradient, and the color argument must be a string representing a CSS <color>, indicating the color the gradient should reach at that offset into the transition.  

_repeat_ Tiles the image in both vertical and horizontal directions.
_repeat-x_ Tiles the image horizontally but not vertically.
_repeat-y_ Tiles the image vertically but not horizontally.
_no-repeat_ Doesn't tile the image. It's used only once.

## Shadows
_shadowOffsetX = float_  
Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.  
_shadowOffsetY = float_  
Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.  
_shadowBlur = float_  
Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.  
_shadowColor = color_  
A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.  