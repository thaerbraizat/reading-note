![html css js](https://miro.medium.com/max/3840/0*crN1sMRpNnApF9Pe.png)
# Html
* canvas tag look like img tag bur without src,canvas has two attributes width and height.
* "When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas,
 it will appear distorted. "
* "The script includes a function called draw(),
 which is executed once the page finishes loading;
 this is done by listening for the load event on the document. This function,
 or one like it, could also be called using window.setTimeout(), window.setInterval(),
 or any other event handler,
 as long as the page has been loaded first."
* canvas tag supports two shapes: rectangles and paths.
* The script includes a function called draw(),
 which is executed once the page finishes loading; this is done by listening for the load event on the document. This function, or one like it, could also be called using window.setTimeout(), window.setInterval(), or any other event handler,
 as long as the page has been loaded first.
## drawing paths
* functions used to draw path
1. beginpath
2. closepath
3. stroke
4. fill
# Css
* we can apply colors to a shape by using fillstyle and strokestyle 
* we can draw transparent shape,by setting the globalAlpha .

## Drawing text
* The canvas rendering context provides two methods to render text:
1. fillText(text, x, y [, maxWidth])
2. strokeText(text, x, y [, maxWidth])
* The text is filled using the current fillStyle
* measureText() that the specified text will be when drawn in the current text style

### Resource
1. [Basic usage of canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)
2. [Drawing shapes with canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
3. [Drawing text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)
4. [Applying styles and colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)
