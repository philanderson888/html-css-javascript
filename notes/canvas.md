# CANVAS

Better for complex scenes, real-time mathematical animations, high-performance elements (filters and ray tracers), and video manipulation.
Canvas is better for real time data
Drawn images cannot be modified by scripting and CSS.
Image types are bitmaps and not easily scalable.
Must add an ID to add the element to the HTML DOM
Must specify which application to run when canvas is clicked
'script' has two functions
Firstly : draw interface
Secondly : process click event


## Sample Canvas Application

```jsx
function drawDiagonal() {
    var canvas = document.getElementById('diagonal'); //creates a css id
    var context = canvas.getContext('2d');
    // Save a copy of the current drawing state to be restored upon exit
    context.save();
    // Move the drawing context to the right and down using transformation
    context.translate(70, 140);
    // Draw the same line as before, but using the origin as a start
    context.beginPath();
    context.moveTo(0, 0);
    context.lineTo(70, -70);
    context.stroke();
    // Restore the old drawing state
    context.restore();
}
window.addEventListener("load", drawDiagonal, true);
<canvas id="diagonal" width="400" height ="400"></canvas>
var myCanvas = document.getElementById('myCanvas01');
var ctx = myCanvas.getContext('2d');                //CRITICAL LINE TO CREATE 
                                                    //JAVASCRIPT CODE FOR CANVAS
ctx.fillStyle = "#FF0000"               // ff RED FULL  00 ZERO  00  ZERO    
ctx.fillStyle = "#F00"                 // same as above, shorter
ctx.fillStyle = "red";                

ctx.fillStyle = "rgb(255, 0, 0)";
ctx.fillStyle = "rgba(255, 0, 0, 0.5)";   // alpha = 0.5 tranparancy
```



USEFUL TO DRAW GRAPHICS WITH JAVASCRIPT


<CANVAS ID="">

CANVAS{
    BORDER:
    
}


JS

VAR CANVAS = DOCUMENT.GETELEMENTBYID('MYCANVAS')

VAR CONTEXT = CANVAS.GETCONTEXT('2D');




RECTANGLE

    CTX.FILLSTYLE="RED"
    CTX.FILLRECT(X,Y,WIDTH,HEIGHT)
    

DELETE EXISTING

    CTX.CLEARRECT(X,Y,WIDTH,HEIGHT)
    

STROKESTYLE  OUTLINE
FILLSTYLE    INTERIOR

PATH : CREATE CUSTOM SHAPE

    BEGINPATH()
    MOVETO(X,Y)
    LINETO(A,B)
    LINETO(C,D)		
    CLOSEPATH()
    
    STROKE		DRAW OUTLINE
    FILL		FILL SHAPE
    
    
LINEAR GRADIENT
RADIAL GRADIENT
PATTERN				SEE CSS CHAPTER ON THESE




CANVAS TRANSFORM

    ROTATE(30DEG)
    
    TRANSLATE(X,Y)
    
    SCALE(X,Y)
    
    
    
    
    



Canvas
http://www.html5canvastutorials.com/	


LINE

    DRAW LINE FROM (X,Y) TO (END-X,END-Y)
    
    line(x,y,end-x,end-y
    
RECT

    DRAW RECTANGLE FROM (X,Y) WITH LENGTH AND WIDTH
    
    rect(x,y, length, width)
    
TRIANGLE

    GIVEN THREE POINTS DRAW A TRIANGLE
    
    triangle (x,y,x1,y1,x2,y2)
    
ELLIPSE

    DRAW AN ELLIPSE CENTRE (X,Y) WITH X-RADIUS AND Y-RADIUS
        
        
background(r,g,b);
stroke(r,g,b);
strokeweight(12);
noStroke();
fill(r,g,b);
noFill();
point(x,y)
arc (x,y,w,h,start,stop)
bezier(x1,y1,cx1,cy1,cx2,cy2,x2,y2)
quad(x1,y1,x2,y2,x3,y3,x4,y4);
image(image,x,y,width,height)
    
    
    
FILL

    FILLS INSIDE THE SHAPE OF THE CHARACTERS WITH FILLSTYLE
    fillStyle   ctx.fillStyle='red' 
    font        ctx.font='90px Verdana'
    fillText    ctx.fillText("text,startx,starty,maxWidth")   FILLS INSIDE TEXT, NO BORDER
STROKE

    STROKES OUTSIDE THE LETTER TO CREATE THE BORDER OUTLINE WITH STROKESTYLE (COLOR) AND LINEWIDTH
    strokeStyle ctx.strokeStyle="green"
    lineWidth   ctx.lineWidth=3;
    font        ctx.font='90px Verdana'
    strokeText  ctx.strokeText('hello',0,0)    STROKES OUTSIDE TEXT, CREATES BORDER
                STROKE AND FILL EXAMPLE
                
                ctx.fillStyle='red';
                ctx.strokeStyle='green'
                ctx.lineWidth=3;
                ctx.font='90px verdana';
                ctx.fillText('Q',50,150);
                ctx.strokeText('Q',125,150);
                ctx.fillText('Q',200,150);
                ctx.strokeText('Q',200,150);
                    PRODUCES http://i.stack.imgur.com/Ypwnz.png



                    
## Canvas

<canvas>
Created using HTML code 
<canvas id="canvasElement" width="480" height="320"></canvas>
Used for gaming where javascript controls the screen
context
moveTo
lineTo
stroke

## SVG Scalar Vector Graphics

<svg>
Used to create images which scale well on any screen at any dimension
context
moveTo
lineTo
stroke

```html
<svg width="200" height="200" style="background-color:#c5ebea">
<circle cx="100" cy="100" r="50" stroke="blue" stroke-width="2" fill="yellow" />
</svg>
<svg width="200" height="200" style="background-color:#c5ebea">
    <ellipse cx="100" cy="100" rx="50" ry="80" stroke="blue" 
                stroke-width="2" fill="yellow" />
</svg>
<svg width="200" height="200" style="background-color:#c5ebea">
    <rect x="50" y="50" width="100" height="100" fill="pink" stroke="blue" stroke-width="2"/>
</svg>
<svg width="200" height="200" style="background-color:#c5ebea">
    <rect x="50" y="50" width="100" height="100" fill="pink" stroke="blue" stroke-width="2" class="transparent" />
</svg>
```


## Canvas Terms

```
addColorStop()             Specifies the colors and stop positions in a gradient object
arc()             Creates an arc/curve (used to create circles, or parts of circles)
arcTo()             Creates an arc/curve between two tangents
beginPath()             Begins a path, or resets the current path
can draw 2D graphics on the fly using javascript
clearRect()             Clears the specified pixels within a given rectangle
clip is like cut
clip()             Clips a region of any shape and size from the original canvas
closePath()             Creates a path from the current point back to the starting point
color picker
container only
context.drawImage(imageElement,x,y,width,height,dx,dy,dw,dh)
context.fillRect (x1,y1,x2,y2)  gives the fill coordinates
context.fillStyle = “colour” determines the fill colour
context.stroke() causes the shape to appear on the canvas
createEvent()             
createImageData()             Creates a new, blank ImageData object
createLinearGradient()             Creates a linear gradient (to use on content)
createPattern()             Repeats a specified element in the specified direction
createRadialGradient()             Creates a radial/circular gradient (to use on content)
document.getElementByID(“...”).getContext(“2d”)
drawImage()             Draws an image, canvas, or video onto the canvas
drawn by Javascript
Dynamically Resize
Expand Image on Hover
fill()             Fills the current drawing (path)
fillRect()             Draws a "filled" rectangle
fillStyle             Sets or returns the color, gradient, or pattern used to fill the drawing
fillText()             Draws "filled" text on the canvas
font             Sets or returns the current font properties for text content
for large number of objects as SVG has to draw each one
for real time data
for small drawings
for small screens/mobile devices
frequent redraw OK
games frequent redraw
getContext()             
getContext(“2d”) returns an object that allows for drawing on the canvas
globalAlpha             Sets or returns the current alpha or transparency value of the drawing
globalCompositeOperation             Sets or returns how a new image are drawn onto an existing image
globalcompositeoperation defines how multiple elements combine on one canvas.  Source-over or destination-over refer to the layering
has no event handler support
has no event listener
has poor text handling capabilities
height             Returns the height of an ImageData object
ID width height
id=”name” width=”400” height = “300”
image map allows links from individual points on a picture
image map links to points on image
is an element to draw or render images
is an empty shell; to draw pixels use JS
is best for graphic intensive games where the image may be re-drawn frequently
is like paint : pixel based
is only a container object
is rendered by pixel
is resolution dependent
isPointInPath()             Returns true if the specified point is in the current path, otherwise false
lineJoin             Sets or returns the type of corner created, when two lines meet
lineTo()             Adds a new point and creates a line from that point to the last specified point in the canvas
lineWidth             Sets or returns the current line width
measureText()             Returns an object that contains the width of the specified text
no events
Note the HTML canvasfeature is only a container: to draw anything you need JavaScript!
produces JPG or PNG
quadraticCurveTo()             Creates a quadratic Bézier curve
rect()             Creates a rectangle
resize
restore()             Returns previously saved path state and attributes
rotate()             Rotates the current drawing
save()             Saves the state of the current context
scale()             Scales the current drawing bigger or smaller
setTransform()             Resets the current transform to the identity matrix. Then runs transform()
shadowBlur             Sets or returns the blur level for shadows
shadowColor             Sets or returns the color to use for shadows
stroke()             Actually draws the path you have defined
strokeRect draws the outline of a rectangle
strokeStyle             Sets or returns the color, gradient, or pattern used for strokes
strokeText()             Draws text on the canvas(no fill)
textAlign             Sets or returns the current alignment for text content
transform()             Replaces the current transformation matrix for the drawing
translate()             Remaps the (0,0) position on the canvas
width             Returns the width of an ImageData object
```