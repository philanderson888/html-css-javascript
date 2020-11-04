# Terms

script async
Script defer
input disabled
input.value
EXEC
find
search
indexOf
lastIndexOf
Apply Call Bind
ctx.moveTo
ctx.textAlign
ctx.strokeRect
ctx.strokeText
ctx.font
ctx.transform
ctx.translate
ctx.lineTo
stroke : needs strokeStyle+font+linewidth+strokeText
strokeText('string',x,y,maxwidth)
textAlign=start/end/left/right/center
fill : needs fillStyle+font+fillText
fillStyle='red'
stroke/fillText('text',x,y,maxWidth)
stroke/fillStyle='green'
lineWidth=3
lambda
d integer
c currency
f fixed
w alphanumeric or _
s white space
S non-white space
worker : w=new worker(abc.js); postMessage();onmessage=fn(event){event.data}
document.querySelector('#myID')
document.querySelectorAll('.myClass')
document.write REPLACES LOADED PAGE
document.write APPENDS TO DOCUMENT OPENED WITH DOCUMENT.OPEN
open NEW WINDOW or NEW DOCUMENT
a:link/hover/active/visited
cursor:crosshair
id.focus ==> gives focus
eval("2+2")   returns 4  don't use
getUserMedia
input type=file capture
manifest file
capabilities
dependencies
prerequisites
publishing the app
permission : execute or full trust
position:fixed to page, absolute to first non-static, relative to previous non-static, static
manifest.appcache : cache always, network never, fallback display if offline
display:inline-flex
flex : left, right, center, stretch
flex : justify
flex : space around
flex : space between
flex-wrap
flex-pack:justify, start, end, center
flex-direction:row,column,reverse
flex-order
grid-columns/rows
grid-template
grid-position
column-count
column-gap
column-rule
word-break:normal/break-all/keep-all
CSS exclusions
exclusions:wrap-flow:both,clear,shape-inside,shape-outside
perspective
transition
animation
@keyframes
canvas : context
CSS gradient : linear, radial, repeating
position:fixed(to page), absolute (to first non-static), relative(to nearest non-static), static
manifest : name, publisher, prerequisites, language, logo, start page
permission : full trust or execution only
appcache : cache (always), network (never), fallback(display if a certain folder goes offline and the app tries to access it)
capture boolean : camera/mic/video/doc
navigator.getUserMedia
navigator.getUserMedia
display:flexbox / inline-flexbox
em
pc
fr
vh 
%
Browser default UNIT
Ajax    Asynchronous Javascript and XML : SEND AND RECEIVE DATA ACROSS WEB 
    USING HTTP/HTML AS THE CARRIER, ALSO CAN DO IT IN A WAY NOT TO 'BLOCK'
    OTHER ASPECTS OF YOUR PAGE
Synchronous STREAM OF DATA : BITS ARRIVE IN SEQUENCE, ONE BY ONE.  WAIT YOUR TURN
Asynchronous  COMMUNICATE WITH DIFFERENT STREAMS OF DATA, ALL DOING THEIR OWN THING
    AND YOU DON'T HAVE TO WAIT FOR OTHER STREAMS TO FINISH
    IN 'PARALLEL'
XML   Extensible Markup Language   STRUCTURED TEXT FILE CONTAINING ROOT TAG <> WITH    

$.AJAX    { ::::: }
$.GET   READ DATA   
$.POST    SEND DATA
PRIMITIVE = IMMUTABLE = CAN'T BE CHANGED 
SEMANTIC TAG : NO FUNCTION : LET COMPUTER KNOW YOUR INTENTION FOR CONTENT AT THAT POINT
SEMANTIC ? GIVE MEANING ..
Video
Audio
<canvas>   FAST JAVASCRIPT DRAWING          PIXEL IMAGE    DOT BY DOT
<fieldset>    Break up page : block unit
<svg>    SCALAR VECTOR GRAPHICS      ?     GENERATED USING MATHEMATICS : SCALE INFINITELY  (SMALL OR LARGE)
<nav>    NAVIGATION : NAVBAR
GEOTAGGING : LOCATION
APPCACHE : ITEMS STORED ON LOCAL MACHINE
LOCAL STORAGE : LARGE ITEMS UP TO 5MB IN SIZE PERMANENTLY ON CLIENT MACHINE
Thursday Morning TERM REVIEW
COOKIE  set expiry    4KB MAX        BOTH CLIENT + SERVER
SESSION COOKIE HAS NO EXPIRY
APPCACHE   =>   INSTRUCTIONS FOR WHICH FILES TO BE CACHED : 3 SECTIONS
1. CACHE ? FILES TO BE CACHED
2  NETWORK ? MUST BE ONLINE (DON'T CACHE) EG LOGIN FILE
3 FALLBACK ?   THIS WEBSITE IS OFFLINE MESSAGE ETC
Manifest.appcache   
JSON   JAVASCRIPT OBJECT NOTATION
{    A:1,B:2,C:”HI”   }
JSON.STRINGIFY   ?  FROM    JSON OBJECT TO STRING
JSON.PARSE       A STRING ? CREATE JSON OBJECT FROM STRING
XML   EXTENSIBLE MARKUP LANGUAGE   ? database with rows, columns, data    IN TEXT FILE
<root>
   <field  att=value>
          <item=value>
  </field>
</root>
CROSS-PLATFORM ? 
WINRT      ?    WIN8 MOBILE PHONE APP
UWP         ?   WIN10       UNIVERSAL APP      (UNIVERSAL WINDOWS PLATFORM)
XAML            XML GUI FOR BUILDING NEW APPS
SDK   SOFTWARE DEV KIT
PUBLISH APP ? WINDOWS STORE
PREREQUISITE     VERSION OF OS AND OTHER APPS WHICH MUST BE PRESENT, OR APP CANNOT BE INSTALLED
DEPENDENCY  
PERMISSION   :   CODE RUNS WITH PERMISSION LEVEL   EITHER   1) EXECUTION ONLY   OR  2) FULL TRUST
WEB WORKER   var w = new Worker('worker.js')
1 message host to worker    w.postMessage('hi')
2. Message worker to host     postMessage('all ok')
3. Receive message worker      onmessage=function(event){//event.data}
4. Receive message host      w.onmessage....
Ajax
XmlHttpRequest   =  xhr   ? OBJECT WHICH  SEND DATA FROM US TO REMOTE SERVER
1      var  xhr = new xmlHttpRequest
2    listen for event data coming back  : TEST  FOR HTTP STATUS 200   &     DATA STATUS==4
            onreadystatechange
3    open('GET',URL,async t/f)
4    send()       
Navigator.geolocation     ?    callback    function(position)
Position.coords.lat/long
Navigator.useragent  =>  
Css Cascading Style Sheet : display only
Attr     
Calc   
Jquery  LIBRARY.   
LOCAL   .MIN.JS   MINIFIED
LOCAL   .JS
CDN  ? CONTENT DELIVERY NETWORK  ?    FAST DELIVERY OF CONTENT WORLDWIDE
DOM
Window.document.body.div...
appendChild  : add to END OF ITEM
insertBefore  : add  eg  as new FIRST ITEM IN LIST
createElement('p')
array
var x = new Array(4)             
var x = [1,2,3,4,”hello”,”sausages”]
push(1)    add at end
pop()    Remove end               var x = myarray.pop()
unshift    Add at start
shift    Remove start
<script>
Var x   ? global   OUTSIDE FUNCTION
Var x   ?  private  INSIDE FUNCTION
Let x = 7    private in CODE BLOCK  { }
CONST
<DIV ID=”X” CLASS=”Y”  Name='z'>
$('#x')           ONE
$('.y')            ARRAY
$('.y')[0]            FIRST AFFECTED ITEM OF CLASS Y
JQuery
Document.getElementById('x')                  ONE
                                        sByClassName
                                        sByTagName('p')
                                        sByName('z')
Document.querySelector('#x')                           ONE
                                            All('.y')                          MANY
<UL>
<LI>
Li:nth-child(0)       FIRST ITEM
Li:first-child
Li:last-child
Li:nth-child(2n+1)  
<ruby>  =   eg ASIAN CHARACTER SETS     <rt>   HAS INFORMATION IN IT   
<rp>      BROWSERS WHICH DON'T SUPPORT <ruby>

MANIFEST FILE : XML WHICH DETERMINES PREREQUISITES EG OS, LANGUAGE, FILES, PATH TO SPLASHSCREEN, LOGO, PUBLISHER

  
  
  
  
  
  

Critical Terms
Overview
app container - An app container is a separate memory space within a system in which an application runs. An app container prevents corruption of the operating system if the application fails for some reason and enables a user to cleanly uninstall the app.
app package - An app package is a file that contains an app’s files and folders. The purpose of an app package is for ease of distribution and deployment.
AppCache - The Application Cache, or AppCache, is an HTML5 feature that enables Web data to be stored locally when a user is offline. AppCache stores resources like images, HTML pages, CSS files, and JavaScript—data that would ordinarily be stored on a server. Because the resources are stored on the client’s hard disk or device, the resources load faster when requested.
application programming interface (API) - An application programming interface (API) is a list of instructions letting a program communicate with another program.
application state - The application state is the phase of a running application at any point in time. For Web applications, the application state is created when the Web browser sends the first request for a Web page to the Web server, and it ends when the user closes the browser.
Cascading Style Sheets (CSS) - Cascading Style Sheets (CSS) is a style sheet language that defines styles for HTML. CSS styles are usually saved in a separate file from the HTML file. This enables you to easily change fonts, font sizes, and other attributes in the CSS file and the changes are reflected across all HTML files that reference the CSS file.
cookies - Cookies are small files that contain information about the user and the Web site visited and are saved on the user’s computer.
debugging - Debugging is the process of detecting, finding, and correcting logical or syntactical errors in an application.
gesture - A gesture is any finger move, which can involve a single finger (one-touch, such as press, tap, press and hold, slide to pan, and so on) or a finger and a thumb (two-touch, such as a pinch and stretch or a turn to rotate).
Hypertext Markup Language (HTML) - Hypertext Markup Language (HTML) is the language used to describe Web pages. It is a markup language, not a programming language, which means HTML uses markup tags such as <body> and <h1> to describe parts of a Web page.
Hypertext Transport Protocol (HTTP) - Hypertext Transport Protocol (HTTP) is the protocol that transfers data on the World Wide Web.
HTML5 - HTML5 is the latest HTML standard and a family of technologies that includes HTML, CSS, and JavaScript. The HTML5 standard won’t be finalized for a few years.
identity permissions - Identity permissions are sets of characteristics that identify an assembly. Identity permissions protect assemblies (compiled code libraries) based on evidence, or credentials, which is information about the assembly that an assembly must have in order to run.
JavaScript - JavaScript is a scripting language that adds interactivity to Web pages.
launcher icon - A launcher icon is a small image that represents an app.
localStorage - localStorage is a JavaScript method that allows users to save relatively large amounts of data from session to session (persistent data), and there’s no time limit as to how long the data exists.
markup language - A markup language is a set of symbols and rules to describe the parts of a markup document, like an HTML Web page.
media queries - A media query is a CSS3 feature that detects the user’s type of screen and sizes the output accordingly.
Metro-style user interface (UI) - A Metro-style user interface (UI) is the UI used in Microsoft Windows 8. The Metro style UI includes features like a clean, uncluttered look and feel, use of the full screen, large hubs (graphical buttons), and a focus on lateral scrolling.
namespace - A namespace is a sort of work area or abstract container for related objects (pages, code, etc.). A single app package can have a lot of functionality. To keep all of the components separated so they don’t conflict, a package defines a namespace.
permission sets - A permission set is a group of permissions. In coding, transparent code executes commands that don’t exceed the limitations of a permission set.
persistent state information - Persistent state information is data that an application needs after the session ends. Many Web applications need to store data (make it persistent) so that users can pick up where they left off when they return to the site.
platform-independent - The term platform-independent describes an application that can run on different desktop and mobile device operating systems, such as Microsoft Windows, Internet Explorer, Windows Phone, Mac OS X, Android, iOS, and Blackberry OS.
scripting language - A scripting language is a programming language that uses scripts and requires no compiler.
session state - The session state is an application’s working set of data. When a user first requests access to an application, the session state is created. The state ends when the user closes the session.
sessionStorage - sessionStorage is a JavaScript method that keeps data only for one session (until the browser is closed), which is also referred to as “per-tab storage.”
touch event - A touch event is the action an application takes in response to a gesture.
touch-screen emulator or simulator - A touch-screen emulator or simulator is an application that imitates a system that only has touch capabilities.
validator - A validator is an application that looks for anything that could cause code to be interpreted incorrectly, such as missing or unclosed tags, an improper DOCTYPE declaration, a trailing slash, deprecated code, and so on.
Windows Runtime (WinRT) - The Windows Runtime (WinRT) is an application architecture, or framework, that sits on top of the Windows 8 kernel. Developers test Windows applications and users run Windows 8 apps within WinRT.
Windows Store - The Windows Store is an online global marketplace for Metro-style apps. Publishing your app for distribution through the store can possibly turn a good idea into a lucrative venture.
World Wide Web Consortium (W3C) - The World Wide Web Consortium (W3C) is the main standards body developing specifications for HTML5, CSS3 and other Web technologies.
application packaging: the process of bundling an application and its resources into an archive format for the purpose of distribution and deployment.
platform: the type of computer or operating system being used. The platforms referenced for the content of this review kit are Windows®, Internet Explorer®, and Windows Phone 7.
permissions: the ability of a particular user to access a particular resource by means of his or her user account. Permissions are grouped into permission sets, and every assembly is assigned a set. The .NET Framework defines some standard permission sets, such as FullTrust (implies all permissions) and Execution (permission to only access the CPU).
credentials: the level of access assigned to a user account. Credentials can be set to Windows Authentication, database authentication, no authentication, or custom authentication.
hosting: the practice of providing computer and communication facilities to businesses or individuals, especially for use in creating web and electronic commerce sites. To become active, an application or service must be hosted within a run-time environment that creates it and controls its context and lifetime.
Images, Audio and Video
attribute - An attribute is a modifier of HTML elements that provides additional information.
audio element - The audio element enables you to incorporate audio, such as music and other sounds, in HTML documents.
canvas element - The canvas element is new in HTML5 and creates a container for  graphics, and uses JavaScript to draw the graphics dynamically.
codec - A codec is a technology used for compressing data.
compression - Compression reduces the amount of space needed to store a file, and it reduces the bandwidth needed to transmit the file.
deprecation - Deprecation is the state of an element or attribute that’s been removed from the list of available HTML elements because its functionality is no longer useful.
doctype - The doctype is an instruction, or declaration, found at the very top of almost every HTML document that associates the document with a Document Type Definition (DTD). When a Web browser reads a doctype declaration, the browser assumes that everything on the Web page uses the language or rules specified in the declaration.
element - An element is the combination of tags and the content they enclose. An element can describe content, insert graphics, and create hyperlinks. A tag pair or an empty tag is called an element.
empty tag - An empty tag is a single tag that doesn’t require an end tag, like <br /> for a line break and <hr /> for a horizontal line.
entity - An entity is a special character, such as the dollar symbol, the registered trademark (a capital R within a circle), and accented letters.
©
©
hello charlie
&
$
figcaption element - The figcaption element adds a caption to an image on a Web page, and you can display the caption before or after the image.
figure element - The figure element specifies the type of figure you’re adding, such as an image, diagram, photo, and so on. This element provides a major benefit: the ability to easily add multiple images side by side.
global attribute - A global attribute is one you can use with any HTML5 element. Examples of global attributes include id, lang, and class, among many others.
nesting - Nesting means to place one element inside another.
raster image - A raster image is an image made up of pixels, such as a photograph. Raster images are most often in JPG format. Other raster file formats that work well on Web pages are PNG, GIF, and BMP.
render - Render means to interpret or reproduce. When a Web browser or mobile device such as a smartphone opens an HTML file, it renders the content of the page.
Scalable Vector Graphics (SVG) - Scalable Vector Graphics (SVG) is a language for describing 2D graphics in Extensible Markup Language (XML). SVG technology is not new, but HTML5 now enables SVG objects to be embedded in Web pages without using the <object> or <embed> tags.
tags - Tags are keywords that help to give an HTML page structure.
valid - Valid means logically correct. If a Web page adheres to the specifications perfectly, it is considered valid.
vector image - A vector image is an image made up of lines and curves based on mathematical expressions. A vector image is an illustration, such as a line drawing. Developers often convert vector file formats from programs like Adobe Illustrator or CorelDRAW, which aren’t supported by Web browsers, into PNG or GIF for Web display.
video compression - Video compression reduces the size of video images while retaining the highest quality video with the minimum bit rate.
video element - The video element enables you to incorporate videos in HTML documents using minimal code.
codec: a technology used for compressing data. Audio and video codec compress and/or decompress digital audio data into different formats to retain the highest quality with minimum bit rate.
data compression: a means of reducing the amount of space or bandwidth needed to store or transmit a block of data, used in data communications, facsimile transmission, file storage and transfer, and CD-ROM publishing.
semantic: the relationship between words or symbols and their intended meanings. Programming languages are subject to certain semantic rules. A program statement can be syntactically correct but semantically incorrect; a statement can be written in an acceptable form and still convey the wrong meaning.
video compression: reduction of the size of files containing video images stored in digital form. If not compressed, 24-bit color video at 640 x 480 pixels would occupy almost one megabyte per frame, or over a gigabyte per minute.
Input Elements
article element - The article element defines a part of an HTML document that consists of a “self-contained composition” that is independent from the rest of the content in the document.
aside element - The aside element is used to set off content that’s related to the current topic but would interrupt the flow of the document if left inline.
autofocus attribute - The autofocus attribute moves the focus to a particular input field when a Web page loads. An example of autofocus is when you open a search engine Web page and the insertion point automatically appears in the input box so you can type search terms without first clicking in the box.
automatic validation - Automatic validation of input means the browser checks the data the user inputs.
client-side validation - Client-side validation is the process of validating user input before submission to the server. A browser is often used to validate user input locally.
datalist element - The datalist element enables you to present the user with a drop-down list of options to select from. Only the options in the list may be selected.
email attribute - The email attribute requires the user to enter an email address into an input field.
footer element - The footer element defines a footer for a document or section, and typically contains information about the document or section, such as the author name, copyright data, links to related documents, and so on.
form input - Form input is the information a user enters into fields in a Web or client application form.
global attribute - A global attribute can be used with any HTML element; in other words, it’s permitted globally.
header element - The header element defines a header for a document, section, or article.
menu element - The menu element presents a list (or menu) of commands, usually with buttons. The W3C prefers that you use the menu element only for context menus, lists of form controls and commands, toolbars, and similar items.
nav element - The nav element defines a block of navigation links. The nav element is useful for creating a set of navigation links as your document’s primary navigation, a table of contents, breadcrumbs in a footer, or Previous-Home-Next links.
ordered list - A list that orders the list entries using numbers, by default.
pattern attribute - The pattern attribute provides a format (a regular expression) for an input field, which is used to validate whatever is entered into the field.
placeholder text - Placeholder text is text displayed inside an input field when the field is empty.
required attribute - The required attribute requires information in a field when the form is submitted.
section element - The section element defines a section in a document, such as a chapter, parts of a thesis, or parts of a Web page whose content is distinct from each other. The W3C specifies uses for the section element to differentiate it from other structure-related elements, mainly that it contain at least one heading and that it define something that would appear in the document’s outline.
semantic markup - Semantic markup is intuitive markup that gives better meaning or definition to several tags so they make more sense to humans, programs, and Web browsers.
server-side validation - Server-side validation is the process of a server validating data received from a user input form.
table - An HTML table contains rows and columns, and is used to organize and display information in a grid format.
unordered list - A list that displays list entries in a bulleted list.
validation - Validation is the process of verifying that information entered or captured in a form is in the correct format and usable before sending the data to the server.
Web form - A Web form is a Web page that provides input fields for a user to enter data, which is sent to a server for processing. From there, the information is stored in a database or forwarded to a recipient.
CSS Key Terms
absolute positioning - Absolute positioning is the placement of an element at a geometric position in the display, relative to the first parent element that has a non-static position.
block flow - Block flow is a positioning method in which an element is separated from other elements by new lines above and below, and fills from left to right the horizontal extent where it appears.
bounding box - A bounding box is an invisible rectangle, the smallest perimeter of which surrounds a word.
Cascading Style Sheets (CSS) - Cascading Style Sheets (CSS) is a style sheet language that defines styles for HTML. CSS styles are usually saved in a separate file from the HTML file. This enables you to easily change fonts, font sizes, and other attributes in the CSS file and the changes are reflected across all HTML files that reference the CSS file.
class - Class is an attribute a Web author uses to provide structure to a document beyond the meaning HTML builds in with elements such as paragraph, header, and so on.
declaration - The declaration is the style for a specific selector. A declaration has a property, which is a style attribute, and a value.
float positioning - Float positioning is the flexible placement of elements, enabling them to move as far as possible either to the right or left; text then “wraps” around the element.
font - A font is a set of characters of a particular size and style.
font-family property - The font-family property can declare either a specific font, like Garamond or Arial, or a wider family that includes many different fonts, such as “serif.”
hidden overflow - Hidden overflow is a feature that makes overflow invisible.
inline flow - Inline flow is a feature that forces no new lines before or after the inlined element, but simply places the element between the content before and after the inlined element.
monospace - Monospace is a type of font family in which each character is the same width. Monospace is often used for technical material such as formulas, numbers, codes, and so on.
rules - Rules are statements that tell Web browsers how to render particular elements on an HTML page or how to apply CSS styles to Web pages.
sans serif - Sans serif is a font style drawn without serifs, such as the Arial font. Serifs are the details at the ends of particular letters; look at the “d,” “p,” and “t” in this sentence for examples of serif characters.
scrolling overflow - Scrolling overflow is a feature that prevents content that can overflow its box from appearing outside the box. The content appears to be clipped.
selector - A selector is a feature that defines which HTML elements will be affected by CSS code. For example, in CSS, the p selector means a particular style will be applied to paragraphs. The general syntax for a selector is selector {property: value}.
visible overflow - Visible overflow is a feature that enables content that overflows it box to appear in the display rather than be clipped or hidden. Visible overflow also writes over the content that follows it.
CSS Box, Flex and Grid Layouts (Chapter 5)
block-level element - A block-level element creates boxes that contribute to the layout of an HTML document. Sections, articles, paragraphs, lists, and images are examples of block-level elements.
border - A border is a colored or transparent line, which can be thin or thick, that surrounds a box. The border is a part of the CSS Box model.
content - Content is whatever is displayed on a Web page, such as text and images. Regarding the CSS Box model, content is text or images contained within a box. You use the border, margin, padding, height, and width CSS properties to modify various parts of the CSS Box model.
flexbox - A flexbox is a type of layout that enables relative sizes and positioning of boxes. Flexbox takes available space into account when defining box dimensions. A box can include child boxes that are flexible by height and width.
flexbox item - A flexible item is a child box. A child box can be flexible or static. The flex property makes child boxes flexible.
Flexbox Box model - The CSS Flexbox Box model is a layout mode for using flexible boxes in user interfaces.
grid item - A grid item is a child element of a grid.
grid layout - A grid layout is a way to structure complex HTML documents using rows and columns to make the design look cleaner and structured.
Grid Layout model - The CSS Grid Layout model is a model for structuring HTML layouts. This model lets you control the design of sections or entire HTML-based documents using CSS3.
grid template - A grid template, an approach to grid layouts, is like an empty table into which data can be flowed. A grid template uses alphabetical characters to represent the position of items in a grid.
inline element - Inline elements are elements designed for laying out text and don’t disrupt the flow of the document. Applying boldface and the new HTML5 mark element are examples of inline elements.
margin - A margin is the outermost edge of a box, providing space between the box and other boxes in an HTML document. Margins are transparent. The margin is a part of the CSS Box model.
media queries - A media query is a CSS3 feature that detects the user’s type of screen and sizes the output accordingly.
padding - Padding is the space between the border of a box and its content. Padding generally takes on the same color as the box’s background color. Padding is a part of the CSS Box model.
parent/child relationship - The parent/child relationship describes how a parent box can contain one or more child boxes. Boxes contained within a parent box are referred to as child boxes. Child boxes inherit attributes applied to parent boxes unless coded otherwise.
user interface (UI) - A user interface (UI) is the portion of a Web site or application with which a user interacts.
vendor prefix - A vendor prefix is a keyword surrounded by dashes, added to the front of a CSS3 property name. The Microsoft Internet Explorer Web browser recognizes the
-ms- prefix. Vendor prefixes help to ensure CSS3 styles work properly in Web pages during the transition from CSS2 to CSS3.
CSS Exclusions, Regions (Chpater 6)
content container - Using CSS Regions, a content container is an area into which content is flowed.
content source - Using CSS Regions, a content source may be one or more blocks of text in the same or a separate HTML document that holds the content you want to flow through a layout. The content is referred to as a “content stream.”
CSS Exclusions - CSS Exclusions are another name for positioned floats.
CSS Regions - CSS Regions are defined areas (regions) of an HTML document where content can flow. Similar to a page layout program, when there’s too much content to fit in one region, the remaining content automatically flows into the next region.
flow-from - The flow-from property specifies one or more content containers.
flow-into - The flow-into property specifies a content source.
hyphenation - Hyphenation is the process of connecting two words with a hyphen mark (-) or breaking words between syllables at the end of a line.
iframe - Iframes are like mini boxes on a Web page that contain external content embedded in an HTML document, as the content source.
multi-column layout - Multi-column layout lets you create columns, divide text across multiple columns, specify the amount of space that appears between columns (the gap), make vertical lines (rules) appear between columns, and define where columns break. You create a multi-column layout using CSS3 properties.
named flow - A named flow is a set of elements taken from the source and to be flowed into a content container.
positioned float - A positioned float is a CSS construct that enables you to position images, text, and boxes anywhere in an HTML document and then wrap text completely around these elements.
CSS Graphical Effects (Chapter 7)  
animation - An animation is the display of a sequence of static images at a fast enough speed to create the illusion of movement.
border-radius property - The CSS3 border-radius property creates rounded corners around layout elements, like headers, footers, sidebars, graphics boxes, and outlines around images. border-radius is a length, which is usually expressed in pixels or ems but can be a percentage. The length is the radius of the circle that defines the “roundedness” of each box corner
drop shadow - A drop shadow is a visual effect in which an object is repeated behind and slightly below itself to create the illusion that the object floats over its background.
gradient - A gradient is a smooth change of colors, either within the same hue, such as from dark green to light green, or starting with one color and ending with a different color, such as starting with blue and ending with yellow.
keyframe - A keyframe is a construct that enables you to change values anywhere within an animation. You can also pause, resume, and reverse animations.
linear gradient - A linear gradient is a horizontal, vertical, or diagonal gradient.
opacity - Opacity is the quality of an object, like an image or rectangle, that does not allow light to shine through; an opaque image is not transparent.
perspective - Perspective, in terms of drawings and illustrations, is the convergence of lines that give the illusion of depth.
radial gradient - Radial gradients start from a central point and radiate color out to the edges of a container.
rotate - To rotate an element turns it clockwise by a specified number of degrees. To rotate an element, you use the rotate() method in CSS and specify the degrees of rotation.
scale - To scale an element is to increase or decrease its size.
skew - To skew an element is to stretch it in one or more directions. To skew an element using CSS, you use the skew() method and provide x-axis and y-axis values, in degrees, to create an angular shape.
SVG filter - An SVG filter is a set of operations that use CSS to style or otherwise modify an SVG graphic. The enhanced graphic is displayed in a browser while the original graphic is left alone.
transform - In HTML5/CSS3, a transform is an effect that lets you change the size, shape, and position of an element.
transition - A transition is a change from one thing to another; in CSS, a transition is the change in an element from one style to another.
translate - To translate an element means to move it, without rotating, skewing, or otherwise turning the image.
transparency - Transparency is reduced opacity.
Web Open Font Format (WOFF) - The Web Open Font Format (WOFF) allows Web developers to use custom fonts instead of being limited to the standard Web fonts. WOFF files are compressed True Type, OpenType, or Open Font Format fonts that contain additional metadata.
Web safe - Web safe refers to a set of standard fonts that are typically located on a user’s computer and render consistently in the majority of Web browsers.
Javascript (Chapter 8)   
callback - A callback is a response to an event, such as a script execution in response to a mouse click.
computer program - A computer program is a recipe we direct the computer to execute that results in a particular display or action.
dynamic application - A dynamic application is one that adjusts and responds to end particular users or user actions.
event handler - An event handler is an optional script or executable that handles input received in a program. Handlers are JavaScript code inside the <html> tags (rather than the <script> tags) that execute other JavaScript code in response to an event.
events - An event is an action that triggers another action to occur.
function - A function is a segment of a program defined and performed in isolation from other parts.
identifier - An identifier is the name of a variable or function. Identifiers cannot be the same as words already used in the language; for example, “if ” has a special meaning in JavaScript statements and is not available as a variable name.
interactivity - Interactivity enables an end user to take an action in an application, usually by clicking a button or pressing a key.
JavaScript library - A JavaScript library is pre-written JavaScript code.
jQuery - jQuery is the leading JavaScript library.
library - A library is collection of resources, like pre-written function code and subroutines, that developers use to create programs. JavaScript builds in a library of useful functions for many common operations.
methods - Methods are JavaScript functions that belong to objects. Methods differ from functions only in that methods are always associated and used with a particular object.
subroutines - A subroutine is a function that returns no value.
validation - Validation is the process of verifying that information entered or captured is in the correct format.
variable - A variable is a symbolic abbreviation, or name, that stands for a piece of data.
 
Animations, Graphics and Data (Chapter 9)   
animation - An animation is the display of a sequence of static images at a fast enough speed to create the illusion of movement.
AppCache - The Application Cache, or AppCache, is an HTML5 feature that enables Web data to be stored locally when a user is offline. AppCache stores resources like images, HTML pages, CSS files, and JavaScript—data that would ordinarily be stored on a server. Because the resources are stored on the client’s hard disk or device, the resources load faster when requested.
canvas element - The canvas element is a drawing area under programmatic control.
cookies - Cookies are small text files that Web sites save to a computer’s hard disk that contain information about the user and his or her browsing preferences.
data type - A data type is JavaScript’s interpretation of the kind of data a program can work with. Data types include string, number, array, Boolean, null, object, and undefined.
encapsulate - To encapsulate is to group data and the methods that operate on it under a single name.
JSON - JSON (JavaScript Object Notation) is a subset of JavaScript, providing a way to store information in an organized, easy-to-access manner.
Local Storage - Local Storage is an HTML5 feature that uses the localStorage method to allow users to save relatively large amounts of data from session to session (persistent data). It is an improvement on data storage using cookies.
parsing - Parsing is a term used to describe analysis of complex information into constituent parts.
recursion - Recursion is a programming technique in which a function calls itself.
XMLHttpRequest API - The XMLHttpRequest API, sometimes abbreviated XHR, enables you to use JavaScript to pass data in the form of text strings between a client and a server.
Advanced Features (Chapter 10)  
accelerometer - An accelerometer is a device that measures acceleration, which is a change in speed or direction over a period of time. The Accelerometer sensor detects forces applied to the device, such as movement (up, down, sideways) and gravity.
Blob - A Blob is a data type that can store binary data, like images or multimedia files.
capacitive touch screen - A capacitive touch screen uses electrodes to sense objects touching the screen. Because the object must have conductive properties, a finger works but something like a stylus does not. Most touch-screen smartphones and computer monitors are capacitive.
civic data - Civic data is location data that’s more easily understood by humans, such as a map or an address like 637 Park Street.
device-independent - A program or interface that runs software that produces similar results on a wide variety of hardware is also called device-independent.
File API - The File API allows a browser or application to upload files from local storage to a remote server without the need for a plug-in.
geodetic data - Geodetic data provides raw location data, such as longitude and latitude, or meters.
Geolocation API - The Geolocation API defines an interface that provides a device’s location, usually using latitude and longitude coordinates. The API exposes the latitude and longitude to JavaScript in a Web page using the geolocation object.
gesture event - A gesture event is a type of touch event triggered by a multi-finger gesture. Gesture events receive event objects that contain touch properties.
local storage - Local storage is persistent data and is useful for things like online to-do lists, contact lists, calendars, and saved shopping cart data. You want this information to be available to the user after the browser closes and the user reopens it at some point. The information is held in persistent memory of Web applications and mobile devices.
platform-independent - The term platform-independent describes an application that can run on different desktop and mobile device operating systems, such as Microsoft Windows, Internet Explorer, Windows Phone, Mac OS X, Android, iOS, and Blackberry OS.
polling - Polling is the process in which a browser contacts a Web server periodically (sometimes constantly) to see if new information is available to present to the user. Technologies such as Comet refresh only a portion of a Web page. Comet and similar “push” technologies introduced polling.
resistive touch screen - A resistive touch screen is made up of several layers, the topmost of which flexes when pressed and pushes into the layer underneath. Sensors detect the pressure, which is how the system knows which part of the screen has been pressed. The touch screens used in hospitals and restaurants are often resistive.
session storage - Session storage is temporary data that’s kept for only one session, until the browser is closed. All of the data in a session is saved in session storage and then erased from session storage when you close the browser tab or window.
touch event - A touch event is the action an application takes in response to a gesture.
touch object - In JavaScript, the touch object detects input from touch-enabled devices.
touchlist - A touchlist references touch objects; the touchlist includes all of the points of contact with a touch screen.
Web Hypertext Application Technology Working Group (WHATWG) - The Web Hypertext Application Technology Working Group (WHATWG) maintains a living HTML specification that includes APIs that were not originally part of the HTML5 specification. These include Geolocation, Web Workers, WebSockets, and File API.
Web Worker API - Web Workers are APIs that allow scripts to run in the background as parallel threads. These background threads can connect to multiple Web pages, fetch real-time data like stock updates, make network requests, or access local storage while the main HTML document responds to the user input like tapping, scrolling, and typing. Web Workers help keep your user interface responsive for users.
WebSocket API - WebSocket is an API that offers full-duplex communication, which is simultaneous two-way communication, through a single socket over the Internet. Developers use WebSockets mainly for real-time Web applications like chat, multiplayer online gaming, and stock quotes.




## CSS Font Awesome
  
http://fontawesome.io/

sectioning root tags
 - body, blockquote, fieldset

@media
 - detect screen size



## Escape Characters

\n  NEW LINE!!!!
\r  carriage return (new line)
\ CAN BE INTERPETED AS AN 'ESCAPE' CHARACTER FOR SPECIAL SYMBOLS
\'
\"
\\

## Image ISMAP

ISMAP is a flag set to TRUE or FALSE inside the <img> tag.  
  <img ismap>  
  If present then this tells the computer that a server-side image map 
  has been created which maps to different parts of the same image, so 
  in order to implement this mapping all that is required is to send the 
  coordinates of the click points to the server as part of the html
  information, in this case as part of the URL information sent.

  Note : relative image coordinates are sent (not absolute page coordinages)

  See W3 Schools ISMAP for working example of this

## Image USEMAP

Usemap is a CLIENT SIDE IMAGE MAP DEFINED HERE
Usemap="#map_region"
<map name="map_region">
  <area shape="rect" coords="0,0,10,10" href="abc.htm" />
  <area shape="circle" coords="10,10,2" ../>
  </map>



## html revision

<section>
  <article>
              <aside>

<tag>   lower case
HTML
XHTML ==> STRICTER VERSION   <tag>  </tag>
<!DOCTYPE html>       HTML5
CSS Cascading Style Sheets
INTERNAL CSS <style>                    </style>
EXTERNAL CSS <link rel="stylesheet" href="style.css">
<head>
<body>
<div>
<div class="container">
<table>
<header>
<footer>
<section>
<aside>
<article>
<video  width="200px"  height="200px" autoplay  controls  muted  ><   src="play.mp4"> 
<audio 
codec
resolution
px
em
pc
fr
vh 
%
Browser default UNIT
Ajax    Asynchronous Javascript and XML : SEND AND RECEIVE DATA ACROSS WEB 
    USING HTTP/HTML AS THE CARRIER, ALSO CAN DO IT IN A WAY NOT TO 'BLOCK'
    OTHER ASPECTS OF YOUR PAGE
Synchronous STREAM OF DATA : BITS ARRIVE IN SEQUENCE, ONE BY ONE.  WAIT YOUR TURN
Asynchronous  COMMUNICATE WITH DIFFERENT STREAMS OF DATA, ALL DOING THEIR OWN THING
    AND YOU DON'T HAVE TO WAIT FOR OTHER STREAMS TO FINISH
    IN 'PARALLEL'
XML   Extensible Markup Language   STRUCTURED TEXT FILE CONTAINING ROOT TAG <> WITH     STRUCTURED SUB-TAGS WHICH REPRESENT ROWS AND COLUMNS OF A DATABASE
    Cross-platform
Cross-platform  
JSON    {
      field:"string",
      field2:3      
    }

$.AJAX    { ::::: }
$.GET   READ DATA   
$.POST    SEND DATA
$   JQUERY
PRIMITIVE = IMMUTABLE = CAN'T BE CHANGED 
HTML 4 : STANDARD HTML   table, p, div
HTML 5 : NEW FEATURES
Div
<header>
<footer>
<article>
<aside>
<section>
SEMANTIC TAG : NO FUNCTION : LET COMPUTER KNOW YOUR INTENTION FOR CONTENT AT THAT POINT
SEMANTIC ? GIVE MEANING ..
Video
Audio
<canvas>   FAST JAVASCRIPT DRAWING          PIXEL IMAGE    DOT BY DOT
<fieldset>    Break up page : block unit
<svg>    SCALAR VECTOR GRAPHICS      ?     GENERATED USING MATHEMATICS : SCALE INFINITELY  (SMALL OR LARGE)
<nav>    NAVIGATION : NAVBAR
GEOTAGGING : LOCATION
APPCACHE : ITEMS STORED ON LOCAL MACHINE
LOCAL STORAGE : LARGE ITEMS UP TO 5MB IN SIZE PERMANENTLY ON CLIENT MACHINE
Thursday Morning TERM REVIEW
COOKIE  set expiry    4KB MAX        BOTH CLIENT + SERVER
SESSION COOKIE HAS NO EXPIRY
APPCACHE   =>   INSTRUCTIONS FOR WHICH FILES TO BE CACHED : 3 SECTIONS
1. CACHE ? FILES TO BE CACHED
2  NETWORK ? MUST BE ONLINE (DON’T CACHE) EG LOGIN FILE
3 FALLBACK ?   THIS WEBSITE IS OFFLINE MESSAGE ETC
Manifest.appcache   
JSON   JAVASCRIPT OBJECT NOTATION
{    A:1,B:2,C:”HI”   }
JSON.STRINGIFY   ?  FROM    JSON OBJECT TO STRING
JSON.PARSE       A STRING ? CREATE JSON OBJECT FROM STRING
XML   EXTENSIBLE MARKUP LANGUAGE   ? database with rows, columns, data    IN TEXT FILE
<root>
   <field  att=value>
          <item=value>
  </field>
</root>
CROSS-PLATFORM ? 
WINRT      ?    WIN8 MOBILE PHONE APP
UWP         ?   WIN10       UNIVERSAL APP      (UNIVERSAL WINDOWS PLATFORM)
XAML            XML GUI FOR BUILDING NEW APPS
SDK   SOFTWARE DEV KIT
PUBLISH APP ? WINDOWS STORE
PREREQUISITE     VERSION OF OS AND OTHER APPS WHICH MUST BE PRESENT, OR APP CANNOT BE INSTALLED
DEPENDENCY  
PERMISSION   :   CODE RUNS WITH PERMISSION LEVEL   EITHER   1) EXECUTION ONLY   OR  2) FULL TRUST
WEB WORKER   var w = new Worker(‘worker.js’)
1 message host to worker    w.postMessage(‘hi’)
2. Message worker to host     postMessage(‘all ok’)
3. Receive message worker      onmessage=function(event){//event.data}
4. Receive message host      w.onmessage....
Ajax
XmlHttpRequest   =  xhr   ? OBJECT WHICH  SEND DATA FROM US TO REMOTE SERVER
1      var  xhr = new xmlHttpRequest
2    listen for event data coming back  : TEST  FOR HTTP STATUS 200   &     DATA STATUS==4
            onreadystatechange
3    open(‘GET’,URL,async t/f)
4    send()       
Navigator.geolocation     ?    callback    function(position)
Position.coords.lat/long
Navigator.useragent  =>  
Css Cascading Style Sheet : display only
Attr     
Calc   
Jquery  LIBRARY.   
LOCAL   .MIN.JS   MINIFIED
LOCAL   .JS
CDN  ? CONTENT DELIVERY NETWORK  ?    FAST DELIVERY OF CONTENT WORLDWIDE
DOM
Window.document.body.div...
appendChild  : add to END OF ITEM
insertBefore  : add  eg  as new FIRST ITEM IN LIST
createElement(‘p’)
array
var x = new Array(4)             
var x = [1,2,3,4,”hello”,”sausages”]
push(1)    add at end
pop()    Remove end               var x = myarray.pop()
unshift    Add at start
shift    Remove start
<script>
Var x   ? global   OUTSIDE FUNCTION
Var x   ?  private  INSIDE FUNCTION
Let x = 7    private in CODE BLOCK  { }
CONST
<DIV ID=”X” CLASS=”Y”  Name=’z’>
$(‘#x’)           ONE
$(‘.y’)            ARRAY
$(‘.y’)[0]            FIRST AFFECTED ITEM OF CLASS Y
JQuery
Document.getElementById(‘x’)                  ONE
                                        sByClassName
                                        sByTagName(‘p’)
                                        sByName(‘z’)
Document.querySelector(‘#x’)                           ONE
                                            All(‘.y’)                          MANY
<UL>
<LI>
Li:nth-child(0)       FIRST ITEM
Li:first-child
Li:last-child
Li:nth-child(2n+1)  
<ruby>  =   eg ASIAN CHARACTER SETS     <rt>   HAS INFORMATION IN IT   
<rp>      BROWSERS WHICH DON'T SUPPORT <ruby>


# CSS Glossary

```jsx
Houdini CSS
CSS Grid and Sub Grid

Background-image:url(image.jpg)
Background-size:cover

Css tricks has a good summary of all css features 

Cursor:pointer shows the mouse hand like when hovering over url 

Display:block
Display : inline-block can produce inline content e.g. menu

Colours at paletton.com

Color 
  #aabbcc hex
  Rgb(1,2,3)
  Rgba(1,2,3,0.5)

Selector by Element, ID, Class, Attribute, Pseudo Class, 
text-decoration
a:visited
a:active
a:link
a:hover
sibling +
sibling ~
input: valid/invalid
input: required/optional
nth-child
Pseudo Class eg nth-child
li:first-child, nth-child,nth-child(2),nth-child(2n+1),nth-child(-n+4),nth-child(4+n)
Pseudo Element :: nth-child
Pseudo Class :active :visited :link :hover
Pseudo Element :: nth-child  ::before  ::after  
::after { content: ' " '  }
::after { quotes :  } 
li { display:inline-block}  // make a list into a horizontal !!!
text-decoration:none/underline
:: before/after{ content: ' addin ' }
:: first-line 
:: first-letter
input:placeholder
text-transform:uppercase
letter-spacing:2px
cursor:pointer;
pointer-events:none
Specificity: 1) Inline 2) ID 3) Class, Attribute, Pseudo Class 4) Element, Pseudo Element

SCSS is an extension of CSS which can be used to extend the language
SASS is an older way of writing concise CSS.  It's fully compatible with all CSS libraries.
LESS stands for Leaner Style Sheets.  LESS is converted to CSS with Less.js

