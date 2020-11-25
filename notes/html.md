## HTML

## Contents

- [Introduction](#introduction)
  - [HTML / CSS / JAVASCRIPT VALIDITY](#html--css--javascript-validity)
  - [Colours](#colours)
  - [What is HTML?](#what-is-html)
  - [HTML5](#html5)
  - [HTML5 Semantic Elements](#html5-semantic-elements)
  - [Javascript](#javascript)
  - [Selecting elements](#selecting-elements)
  - [Creating Elements](#creating-elements)
  - [Declaring variables](#declaring-variables)
  - [Data types](#data-types)
  - [JSON](#json)
  - [SetTimeout and SetInterval](#settimeout-and-setinterval)
  - [HTML Continued](#html-continued)
  - [Rarer elements](#rarer-elements)
  - [HTML5 changed elements](#html5-changed-elements)
  - [SVG](#svg)
  - [DATA-](#data-)
  - [HTML Forms](#html-forms)
  - [Input Elements](#input-elements)
  - [Input Attributes](#input-attributes)
  - [Regex](#regex)
  - [Output Elements](#output-elements)
  - [Tables](#tables)
  - [Table](#table)
  - [abbr](#abbr)
- [innerHtml](#innerhtml)
- [data-*](#data--1)

## Introduction

  HTTP IS A PROTOCOL (LANGUAGE) USED TO SEND DATA ACROSS THE WEB

  create a page

    HEADER (METADATA)   SEND PAGE ACROSS WEB

    BODY OF PAGE (HTML DATA)

  WEB SERVER ===> 'RENDER PAGE' ==>  SEND HTML TO CLIENT  ==> USE 'BROWSER' TO 
            DISPLAY HTML TO USER

  HTML  
    <>
    PLAIN TEXT

  DOM STRUCTURE Document Object Model

  WINDOW

    ==> DOCUMENT

      ==> HTML

        ==> HEAD

          METADATA

        ==> BODY

          <DIV CLASS="CONTAINER">

            <BUTTON>

  <img src="mypic.jpg">

    img   Element
    src   Attribute
    mypic.jpg Value

  
  
Central Organisations

  w3.org    WWW Consortium

  ietf.org  INTERNET ENGINEERING TASK FORCE

      RFC REQUEST FOR COMMENTS
  
            
  
Standards

  http://javascript.crockford.com/code.html
  
  

<meta>

  <head>
    <meta>

      METADATA IS data about data

        critical data concerning your web page

      <meta charset="utf-8">
          <meta http-equiv="X-UA-Compatible" content="IE=edge">
          <meta name="viewport" content="width=device-width, initial-scale=1">        
  
      UTF-8  =   'UNICODE'  DEFAULT "ENCODING"  WAY TEXT IS CREATED/STORED

        ASCII ((COMMON ENGLISH CHARACTERS ONLY))

      UTF-16    ABLE TO DISPLAY CONTENT FROM ANY LANGUAGE IN WORLD
          WITH ANY CHARACTER 

## HTML / CSS / JAVASCRIPT VALIDITY

  caniuse.com

    FEATURE IS CURRENT/VALID ==> SHOULD I USE IT???    
    
        

## Colours

#eee;
#eeeeee;
rgb(R,G,B);
rgba(R,G,B,Alpha)
CMYK

## What is HTML?

It is a language used to transmit information across the internet from one machine to another
Data is transmitted from one machine (client) to another (server), and vice-versa.
HTML data is split into two parts : the header information which tends to be INVISIBLE then the body information which produces the visible page.
HTML is PLAIN TEXT
HTML can be EDITED WITH ANY TEXT EDITOR
HTML souce code can be VIEWED FOR ANY PAGE (Inspect Element on any web page)

What is the structure of HTML?

HTML uses something called the DOM (Document Object Model) model to produce data which can be viewed (rendered) on a page.  Data is stored on the server in text files called .htm files and then when it is sent to the client, the browser is a program which takes this data and produces output for the viewer to see.

Who's in charge of the development of HTML?

W3C the World Wide Web Consortium is a group of companies and organisations which steer the development of HTML and other web-related standards.

Website at https://www.w3.org

Follow at https://twitter.com/w3c

Where are the best places on the web to investigate and learn HTML?

W3C Official Site 
Mozilla HTML reference 
W3Schools to learn
CodeCademy to learn with dynamic editor
Code.org

XHTML is a stricter form of HTML which enforces 1) lower case tags 2) all start tags must have a closing tag etc..

Building A Basic Web Page

<tag></tag>

Used to open and close all documents within an HTML page
Every opening <tag> must have a corresponding </tag> closing tag
Some tags are 'self closing' such as <input />
<!DOCTYPE html>

<html>

<head>

<meta>

'meta' data is DATA ABOUT DATA so the <meta> tags will hold information about the web page and some of the data within it
<meta charset="UTF-8">  where UTF is a 2-byte character set used to represent all of the languages in the whole world.  Using it we can represent any character in any language which is quite useful!!!

<title>
Goes within <head>
Note that "title" is an attribute that can be used to generate hover text also eg 
<span title="display this text on hover">Hover Over Me</span> produces Hover Over Me 
<body>
Defines visible part of document

HTML tags
See Entire List Of HTML tags At These Locations

Learning Material
http://www.w3schools.com/tags/
Official Reference
https://developer.mozilla.org/en-US/docs/Web/HTML/Element
W3C Official Reference
http://w3c.github.io/html-reference/elements.html#elements
CanIUse.Com

Use to see if a particular feature is supported by a particular browser
Rendering engines : be aware different browsers 'render' or display data using different mechanisms called 'rendering engines'.  
https://en.wikipedia.org/wiki/Comparison_of_layout_engines_(HTML)
Discussion : Blink is a newer engine run by Google, Opera and Samsung https://en.wikipedia.org/wiki/Blink_(web_engine)
<strong>

<em>
<small>

<hgroup> contains <h1>...to <h6> tags

What is the DOM Model?
Document Object Model

It is a clear hierarchy of every object laid out correctly and finding its place on the page, so we can locate every item uniquely  using a simple hierarchy system. 
WINDOW ==> DOCUMENT ==> HTML ==> BODY ==> ELEMENT ==> ATTRIBUTE ==> VALUE
<div>

## HTML5

HTML5 Structure Elements 

Nav
Header
Section
Article
Aside
Footer

## HTML5 Semantic Elements

These elements may not actually DO ANYTHING but they convey MEANING to the BROWSER PROGRAM and possibly to the END USER also.
A good example will be <header> or <footer> which don't actually do anything but can be used to clearly mark where the page header and footer go.

List Of HTML5 Semantic Elements Below:

<article>    Defines an article
<aside>    Defines content aside from the page content
<details>    Defines additional details that the user can view or hide
<figcaption>    Defines a caption for a <figure> element
<figure>    Specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.
<footer>    Defines a footer for a document or section
<header>    Specifies a header for a document or section
<main>    Specifies the main content of a document
<mark>    Defines marked/highlighted text
<nav>    Defines navigation links
<section>    Defines a section in a document
<summary>    Defines a visible heading for a <details> element
<time>    Defines a date/time
http://www.w3schools.com/TAGS/tryit.asp?filename=tryhtml5_time
Outlining : automatically splitting page up into sections eg at https://gsnedders.html5.org/outliner/ 

## Javascript
      
Async

    <script async src="abc.js"></script>    

Immediate

    <script>alert('hello')</script>     ALERT STRAIGHT AWAY

Defer

    <script defer    DON'T RUN SCRIPT UNTIL PAGE LOADED


  
## Selecting elements

  give element a 
      ID    ID="X"
      CLASS   class="green"
      
  or select by TAG  

  document.getElementById(x)
  document.getElementsByClassName('green')
  document.getElementsByTagName('h3')

  document.querySelector('#x')                 (all) as well

  $('#x').      ID
  $('.green')   CLASS

Amending Elements

  document.getElementById('x').innerHTML = "<p>HI</p>"

                              .width="200px"

                              .setAttribute("width","200px");
  

## Creating Elements

var text_node = document.createTextNode("some text");
var paragraph_node = document.createElement('p');
paragraph_node.appendChild(text_node);
document.body.insertBefore(paragraph_node,document.getElementById('start_point'));

## Declaring variables

  var

    Global : all functions

      <script>
        var x=1;      global

    Local : within function

      function y{}{
        var z=2;      LOCAL INSIDE FUNCTION   
      }
    
      // z not visible HERE

  
    MISTAKE :    X=7;    (NO VAR)  ==> NO ERROR

    use scrict;   FIRST LINE OF CODE ==>  forces var declaration

  let 

    within a BLOCK OF CODE EG A FOR LOOP 

    let t = 22;     VALID ONLY IN THE LOCAL CODE BLOCK

  const
    const c = 15;     FIXED

  scope = visibility of element

  

## Data types

  CAN REASSIGN A VARIABLE LIVE

    var x = 1;
    var x= "hi";
  
  String
  number
  Boolean     var x=true
  Null      var x=null
  Undefined   var x;
  Date      var d = new Date("25 Sept 2017 08:17")
        var d = new Date()      NOW

      getDate() 22 => 22nd of the month
      getDay()  3 =>  Monday 1   Wed 3    Sunday 7 (or zero)
      getMonth()  zero based counting 0=jan 1=feb dec=11
      
  Object    same as JSON   
    
      {
        a:1,
        b:"hi",
        c: { z:22 }

      }

  Array

      var myArray=[1,2,3];
      myArray.push()    add to end
      myArray.pop()     from end
      
              var z=myArray.pop()  

      myArray.shift()   remove from start
      myArray.unshift() add to start
  

  Declare a variable

        var x;    

          DECLARED BUT "UNDEFINED"

        var x="1",y=1,z=3;

      

  ## JSON 

    var y = {
      a:1,
      b:"some string"
    }

    y.a
    y.b
    y.b.length
    y.b["length"]

    EXTEND AN OBJECT (ADDING ATTRIBUTES)

    y.newProperty=16;

    y.prototype.newPropertyB = 77;     // ADD NEW CLASS VALUE TO STRUCTURE

Input/Output

  alert('hi')
  confirm('are you sure')     
  prompt('what is your name',"no name")

    
onload() event

  <body onload="dothis()">   CAN BE USED TO RUN A FUNCTION AFTER PAGE LOADS

  OR

  $(document).ready(function(){
      // code 
  });

Validation

Input can be validated eg isNaN() can be used to test if an item is a number or not.


## SetTimeout and SetInterval

setTimeout      SETS A DELAY

  setTimeout(doThis,after_this_delay);

setInterval     REPEAT LIKE A CLOCK

  setInterval(doThisFunction,repeat_function_every_x_milliseconds);

Creating elements eg an image

document.createElement('img');
img.src
img.width
img.height
document.body.appendChild(img)

    
## HTML Continued

<audio>
play audio files natively from within HTML browser without any other plugins
<video>
play video files natively from within HTML without any other plugins like flash or silverlight
Geolocation 
Detect position of phone on the globe
Canvas
Draw images using Javascript
CSS Media queries : use CSS to detect screen size and adjust display accordingly
Modernizr
https://modernizr.com/docs/#what-is-modernizr
 if (Modernizr.awesomeNewFeature) {
    showOffAwesomeNewFeature();
  } else {
    getTheOldLameExperience();
  }
Application Storage
Session Storage
Local Storage

<input> tag to connect to camera, video and microphone

input type="file" accept="image/*;capture=camera"
input type="file" accept="video/*;capture=camcorder"
input type="file" accept="audio/*;capture=microphone"

navigator.getUserMedia Javascript function to access camera, video and microphone
https://www.html5rocks.com/en/tutorials/getusermedia/intro/
function hasGetUserMedia() {
  return !!(navigator.getUserMedia || navigator.webkitGetUserMedia ||
            navigator.mozGetUserMedia || navigator.msGetUserMedia);
}

if (hasGetUserMedia()) {
  // Good to go!
} else {
  alert('getUserMedia() is not supported in your browser');
}
navigator.getUserMedia

https://www.html5rocks.com/en/tutorials/getusermedia/intro/

Examine working example from your phone at this URL : goo.gl/dUsrzH

## Rarer elements

<command>
<mark>
<time>
<meter>
<progress>
<details>
Provides a drop-down for content
http://www.w3schools.com/tags/tryit.asp?filename=tryhtml5_details
<time>



## HTML5 changed elements

A few elements have CHANGED THEIR MEANING

<b>
WAS : bold
NOW : use CSS for bold effect
<i>           
WAS : italic
NOW : use CSS for bold effect
<u>
WAS : underline
NOW : use CSS for underline effect

Images

Raster Image (with pixels)

Vector Image (scalable)

<img>

<figure>

<figcaption>

<alt>

Used to display alternative text when the image cannot load for some reason

## SVG

Better for static images and high-fidelity documents for viewing and printing.
Objects are part of the Document Object Model (DOM); they can be modified by scripting and CSS at any time.
Vector graphics are scalable.
Sample Game
https://msdn.microsoft.com/en-us/library/gg589521?f=255&MSPPError=-2147217396


## DATA-

CAN ADD CUSTOM DATA- ATTRIBUTES LIKE ID FIELDS

DIV DATA-NAME="X"

    $('DIV[DATA-NAME="X"]')



## HTML Forms

- Input Types
- Input Attributes
- Placeholder
- Required
- Pattern
- Tables
- Definition Lists

Forms
Document Object Model

## Input Elements

Text Field (type="text")
Number Field (type="number")
Pattern
Date Field (type="date)
URL (type="url")
Email (type="email")
Password (type="password")
Datalist - Used to provide 'autocomplete' as users find an item within a pre-determined list
url    For entering a URL. It must start with a valid URI scheme, (for example http://, ftp:// or mailto:).
tel    For entering phone numbers. It does not enforce a particular syntax for validation, so if you want to ensure a particular format, you can use pattern.
email    For entering email addresses. By default it will only take one, but if the multiple attribute is provided, a comma separated list of email addresses is valid.
search    A text input field styled in a way that is consistent with the platform's search field.
number    For numeric input, can be any rational integer or float value.
color    For choosing colors.
range    For number input, but unlike the number input type, the value is less important. It is displayed to the user as a slider control.
datetime    For entering a date and time value where the time zone is provided as GMT.
datetime-local    For entering a date and time value where the time zone provided is the local time zone.
date    For entering a date (only) with no time zone provided.
time    For entering a time (only) with no time zone provided.
week    For entering a date that consists of a week-year number and a week number, but no time zone.
month    For entering a date with a year and a month, but no time zone.

## Input Attributes

placeholder

required



## Regex

used to validate the user input against a very specific arrangement of letters, numbers and characters specified inside the pattern /... / string
pattern=“\d{3}-\d{4}” forces ddd-dddd where d stands for any alphabetic character 

let this site teach you (https://regexone.com/)

then move on to more advanced playing around with regular expressions here - http://regexr.com

  \s    whitespace

  \d  number

  \w  word (character)

  ^ starts with

  $ ends with

  a*    means 0 or more instances            aaaa OK

  a+    means 1 or more instances

  a?    means 0 or 1 instance 
  
  [^9]   not 9

autocomplete
 specifies if an element may have autocomplete enabled

autofocus
 this element will get the focus when the page loads

list - refers to <datalist>

max / min eg of number element

maxlength of input element

Validation Of User Form Input

Lab : Create a form and validate different types of input
New Form Elements in HTML5

What do the new form elements (progress, meter, datalist, keygen, and output) add to a web page? 
Progress is a control the shows the status of a task being completed such as a file being uploaded. 
Meter is used for scalar measurement within a known range such as temperature or weight measurement. 
Datalist is used to show a list of options; it is used with the new list attribute for the input element. 
Keygen is a control for key-pair generation. 
The output control displays the result of a calculation; an example would be the sum of the values of two input elements. (NOTE: These are not supported in IE9)

## Output Elements

## Tables

<table>
<caption>
<thead>
<tbody>
<tfoot>
<tr>
<td>
<col> for styling
<colgroup> for styling
 

Alternative To Table - Definition List

Note : Can be called either Definition List or Description List
<dl> Definition List
<dt> Definition Tag
<dd> Definition Detail


## Table

- <colgroup> <col span="2" style="background-color:red"> <col style="background-color:yellow"> </colgroup>
- border-collapse avoids having double borders for overlapping elements
- caption caption-side:top/bottom etc
- caption defines the title of the table, outside it
- cell can have HTML within it eg <p> <table>,<ul> which is incredible!!!!
- cellpadding provides whitespace within cell <table border="1" cellpadding="10">
- cellspacing provides space around cell <table border="1" cellspacing="0">
- col defines formatting for a column or group of columns in colgroup
- frame <table frame="border"> <table frame="box">
- frame above/below/vsides/hsides/lhs/rhs eg <table frame="hsides">
- frame missing <table frame="void">
- header row <tr><th>Header 1</th><th>Header 2</th></tr>
- padding between a border and content
- rows may be grouped into header, body, footer by the THEAD TFOOT and TBODY tags
- text-align left/right/center/justify
- thead tbody tfoot can be styled by CSS eg <thead><tr><th>Month</th><th>Savings</th> </tr></thead>
- vertical-align sets the heght of text in the box eg top/middle/bottom



## abbr
    
    abbr has full name on mouseover
    

# innerHtml

Can be used to read the contents of a div which are being displayed

```js

// https://www.w3schools.com/tags/att_data-.asp 

<!DOCTYPE html>
<html>
<head>
<script>
function showDetails(animal) {
  var animalType = animal.getAttribute("data-animal-type");
  alert("The " + animal.innerHTML + " is a " + animalType + ".");
}
</script>
</head>
<body>

<h1>Species</h1>
<p>Click on a species to see what type it is:</p>

<ul>
  <li onclick="showDetails(this)" id="owl" data-animal-type="bird">Owl</li>
  <li onclick="showDetails(this)" id="salmon" data-animal-type="fish">Salmon</li>  
  <li onclick="showDetails(this)" id="tarantula" data-animal-type="spider">Tarantula</li>  
</ul>

</body>
</html>
```

# data-*

This can be used to embed data inside an HTML element which can be read at any time

```js
// https://www.w3schools.com/tags/att_data-.asp 

<!DOCTYPE html>
<html>
<head>
<script>
function showDetails(animal) {
  var animalType = animal.getAttribute("data-animal-type");
  alert("The " + animal.innerHTML + " is a " + animalType + ".");
}
</script>
</head>
<body>

<h1>Species</h1>
<p>Click on a species to see what type it is:</p>

<ul>
  <li onclick="showDetails(this)" id="owl" data-animal-type="bird">Owl</li>
  <li onclick="showDetails(this)" id="salmon" data-animal-type="fish">Salmon</li>  
  <li onclick="showDetails(this)" id="tarantula" data-animal-type="spider">Tarantula</li>  
</ul>

</body>
</html>
```


## CODEC

SOFTWARE DELIBERATELY MATCHING A PARTICULAR AUDIO/VIDEO FORMAT TO ENABLE PLAYBACK

## figure and figcaption
    
```html
<figure>
  <figcaption>Several images</figcaption>
  <img src=".." />
  <img src=".." />
  <img src=".." />
```


## form

```
    <input     autofocus PAGE LOAD : CURSOR BLINK IN THIS FIELD
              SO USER TYPES, ALREADY IN THIS BOX

          readonly  date : view only (can't select) 

          disabled  <button GREYED OUT, CAN'T PRESS>

          tabindex  tabbing order

    visibility:hidden KEEP IN DOM; JUST NOT VISIBLE   

    display:none    REMOVE FROM DOM 
              
  z-index     -1  bottom layer
        0 mid layer
        1 top layer
        10  top of all
  
  <wbr>   WORD BREAK               : word will break if it is at end of line

  autocomplete    (in form) BROWSER WILL BE ALLOWED TO USE USER DATA
            TO PRE-COMPLETE FIELDS
  
  datalist : option box (can type)

  

  <form method=GET/POST action="URL" target=_blank=NEW,_self SAME FRAME
            ,_parent FRAME,top SAME WINDOW

    
    onSubmit="return fnValidate()"

        
    <button type="button"      NOT RELATED TO FORM
           "submit"     SUBMIT FORM
           "reset"      RESET FORM

    
    <script>
    function fnValidate(){
      //CODE
      return true/false
    }

    <script>
    function fnValidate(){
      //CODE
      myform.submit();    SUBMIT
    }

  <input required

    required="required"
```
## regex

```html
<input pattern="[0-9]{5}" />      FORCES 5 NUMBERS
<input pattern="[a-zA-Z]{2}" />   2 alpha
```

```js
// any character alphanumeric a-z and 0-9
\w      
// white space
\s    
// non-white space
\S  
// first search result
var myregex = "/searchterm/"
// global search with multiple hits
var myregex = "/searchterm/g"         
```