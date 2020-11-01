## Javascript 

Adding Javascript To A Page

Variables

  var
  numbers
  strings

Communicating With The User

Alert
Confirm
Prompt

## Events

event Listener
addEventListener
onclick
event handler
onLoad

Example

  show/hide data with display:none/visible 

  set CSS with document.body.style.backgroundColor= "green";

## DOM Model : Finding Elements

  document.getElementById('id')

## jQuery 

  $(document).ready(function(){});
  $('selector').doSomething

Using Javascript To Alter HTML DOM Elements

innerHTML
createElement
var newRadioButton = document.createElement("<INPUT TYPE='RADIO'
NAME='RADIOTEST' VALUE='First Choice'>")
insertBefore/After
document.body.insertBefore(newRadioButton);
appendChild
Hide an element with display:none
document.getElementById(“hide”).style.display:none;

Graphics : Bringing It All Together : Chapter 5

## Animations

setTimeout()
setInterval()
animate
Animation can be done with CSS Keyframes
Animation can also be done with jQuery animate() method
http://api.jquery.com/animate/
See examples in section 4.3
Working With Images, Shapes and other Graphics

createElement to place images on a page
Canvas manipulation with Javascript

canvas.getContext
Example
Canvas clock
Animated box
AJAX : Send and Receive Data

XMLHttpRequest
Complex Javascript Objects 
JSON
JSON.parse
JSON.stringify

Parsing Data

String.split(';');

See example in section 4.4

Loading and saving local text files

Validation Of File Type before loading



## Storage

HTML is a STATELESS PROTOCOL

  it does not have any 'memory' of previous page visits

Persistence = STORING DATA BETWEEN CLICKS

Storing Data Between Clicks - The 'State' Of The Application or Session

Persistence is the ability to store data

Data can be stored on the SERVER and the CLIENT!

HTML

  Stateless protocol : does not have any inherent 'memory' of previous page visits

Look at

  1. Cookies
  2. Session Cookies
  3. Application State
  4. Local Storage

  
## Cookies

    SMALL TINY PIECES OF DATA
    
    4kb max

    SENT WITH EVERY PAGE REQUEST 

    DATA ACCESSIBLE BOTH BY CLIENT AND SERVER

      document.cookie = "username=John Doe";

      document.cookie = "username=John Doe; 
            expires=Thu, 18 Dec 2013 12:00:00 UTC";

      SESSION COOKIE HAS NO EXPIRY DATE; VALID FOR THIS SESSION ONLY

    ((COOKIE/SESSION DATA ==> VALID FOR ONE USER ONLY))

    Example at http://jsfiddle.net/user/philanderson888/fiddles/

  ## Local Storage

    FOR LARGE FILES WE WANT A WAY OF STORING DATA ON LOCAL CLIENT MACHINE

    5MB PERMANENTLY ON CLIENT

    localStorage.setItem("lastname", "Smith");

    localStorage.lastname

    localStorage.getItem("lastname")

  ## Session Storage

    
    same as local storage, destroyed after session

    sessionStorage.setItem("lastname", "Smith");

  Browser Cache (temporary internet files)

    Files downloaded eg CSS, Javascript can be stored in client cache for
        later use

## Cookies

Cookies are small text files which can be used to transmit data between the client and the server which reflect the state of the session or application.
Small file size (4kb)
Sent with every HTTP request
Can be accessed by both client and server code

Cookies are tiny (4kb max) pieces of text data

They are SENT WITH EVERY HTML REQUEST

create with

document.cookie="username=Phil";

  ((store data as key/value pair))

  IF NO EXPIRY DATE ==> SESSION COOKIE : DELETED WHEN YOU FINISH
    USING THIS SITE

expires="18 Dec 2017";

  THIS COOKIE NOW LAST UNTIL THAT DATE




## HTML5 localStorage

Local storage is the ability to store files and data permanently on the client machine.  
This is fully persistent ie it has no time span after which the data will expire, 
so in that sense the data is permanent although if the client clears their cache and temporary 
storage areas out which they are more than welcome to do at any stage, the data will be erased.
Can only be accessed by client browser code
Can timestamp and purge items from local storage cache in order to manage space effectively
Lab - Code on PDF : does your browser support local storage???

Up to 5MB max

localStorage.setItem("firstName","phil");
            

Get data (next time)

  localStorage.getItem("firstName");   ==> return "phil"

Shorten this

  localStorage.firstName   ==> return "phil"

HTML5 Session Storage

Same exists just for one session

sessionStorage.setItem..
              .getItem..    same syntax

Note : BROWSER CACHE WILL ALREADY STORE EG IMAGES, GIF, STYLESHEETS, JS, FROM 
  YOUR SITE ANYWAY ***********

Application State

The data pertaining to the application as a whole for all users

## Session State

The data pertaining to one user after they log in, relevant for that user for that logged in 'session' until they either log out or they stop using the application in which case after a certain time span the session will automatically log them out and the session data will cease to exist.
Storing Data Permanently On The Client Device

## Touch

Gestures
touchstart
touchmove
touchend
touchcancel
touch object
touchlist
touches
targetTouches
changedTouches

addEventListener

```html
<div onclick='alert("you clicked");'>click once</div>   //INLINE
<div id="clickMeTwice">click twice</div>
<script>
document.getElementById("clickMeTwice").addEventListener("dblclick", fnDblClick);
function fnDblClick() {
    document.getElementById('clickMeTwice').innerText = "You double clicked ";
}
</script>
```

gesturestart
scale
rotation
gesturechange
gestureend


Geolocation
API
getCurrentPosition
watchPosition
Example in Textbook

## Web Workers

Isolated threads - in a different environment to the DOM so therefore cannot access DOM elements
passing a message to a Web Worker
receiving a message from a Web Worker

## Web Sockets

Full-duplex two-way communication through a channel over the internet ws:// or wss:// similar to HTTP but not using headers for every request so very lightweight
Uses : real time eg chat applications, gaming, live stocks and share updates
declare a socket
var mySocket = 'ws://mysite.com';
var mySecureSocket = 'wss://mysecuresite.com';
onopen()
onmessage()
onclose()

HTML File API

Input type=file (one)
Input type=filelist (array)
Input type=blob
Filereader means to read a text file line by line

Talking To Your Device's Hardware 

  Accessing the camera
  Accessing the GPS
  Accessing the accelerometer
  Host Process

Touch Interface

Events

  Focus/Blur
  Select
  Resize

Keyboard Events

  KeyPress
  KeyDown
  KeyUp
  shiftKey/ctrlKey/altKey
  charCode : Keyboard Letters, Numbers and Characters : KeyPress
  scanCode : Special Keys like Escape : KeyUp/Down
  http://javascript.info/tutorial/keyboard-events

Mouse Events

  mouseMove
  mouseDown
  mouseUp
  mouseEnter
  mouseLeave
  mouseOut
  click
  dblClick

Finger Events : Gestures

  TouchStart
    Finger is placed on the screen

  TouchMove
    Finger is dragged across screen

  TouchEnd
    Finger is removed from screen

  Testing Finger Events : Using An Emulator
    Hold down shift in these emulations to simulate multiple finger touches
    http://cdn.rawgit.com/hammerjs/touchemulator/master/tests/manual/hammer.html
    http://cdn.rawgit.com/hammerjs/touchemulator/master/tests/manual/leaflet.html

## AJAX

AJAX demos are in the Showcase folder

  Delete up to 10

  Ajax 10

  Serialize  : Ajax 11

  Live AJAX call : Ajax 12

AJAX USING XMLHTTPREQUEST

    request = new XMLHttpRequest();       CREATE REQUEST OBJECT

    request.open('GET',url,true);
      // Get = read data
      // true = asynchronous

    request.onload=function(){
      callback(request.responseText);
    };
    request.send(data);   // Fire off request

   request.onreadystatechange = function() {
        if (this.readyState == 4 && this.status == 200) {
          document.getElementById("demo").innerHTML =
          this.responseText;
        }
    };

Book example

function loadJSON(url, data, callback) {
    var xhr = new XMLHttpRequest();
    xhr.open("GET", url, true);
    xhr.onload = function() {
        callback( JSON.parse(xhr.responseText) );
    }
    xhr.send( JSON.stringify(data) );
}
loadJSON("my.json", { id : 1 }, function(response) {
    setTitle(response.title); 
});

AJAX USING JQUERY

  $.ajax({
      method: "GET/POST",
      url: "some.php",
      data: { name: "John", location: "Boston" }
  })
  .success(function( msg ) {
        alert( "Data Saved: " + msg );
  });
    

  $.GET

    $.get("URL",function(data){
      // handle data
    });
  

  $.POST

    $.post("URL",dataOUT,function(dataIN){
      // handle dataIN
    });

  $.LOAD

    $('#divID').load("URL");
            DATA ==> PAGE ELEMENT

    

Parsing Data

var text="this;is;some;long;list;of;items";
var list=text.split(';');
for(var i = 0; i < list.length;i++){
  console.log(list[i]);
  console.log(list[i].trim());
}



## Geolocation

  navigator element can LET US KNOW OUR COORDINATES ON PLANET

    navigator.geolocation.getCurrentPosition(function(position){

    });

      1. ASK FOR POSITION
      2. WHEN DATA COMES BACK, RUN A FUNCTION (CALLBACK)
        function(position)    POSITION = OUR DATA 
      3. EXTRACT COORDINATES
          position.coords.longitude


## touch events

  $('mycanvas').addEventListener('click'
                                       'mouseover'
                                       'touchstart    FINGER HITS
          touchmove     DRAG FINGER
          touchend    LIFT FINGER
            ((prefer touchend not touchcancel))

  touch target    item event happens to 

    
  TOUCHES     ARRAY OF MULTIPLE FINGERS ON SCREEN

  TARGETTOUCHES   ARRAY OF FINGERS INVOLVED IN THIS EVENT

  9mm optimal
  7mm min


```html
<fieldset>
    <h1>Javascript - innerText/innerHTML</h1>
    <button type="button" onclick="fnChangeText()">Change Text</button>
    <div id="amendHTML">hi</div>
    <script>
        function fnChangeText() {
            document.getElementById('amendHTML').innerText += "<h1>I am changed</h1>";
        }
    </script>
</fieldset>

<fieldset id="setMyWidth">
    <h1>Javascript - setAttribute</h1>
    <button type="button" onclick="fnChangeText2()">Change Text</button>
    <div id="amendHTML2">hi</div>
    <script>
        function fnChangeText2() {
            $('#amendHTML2').html("<h1>I am changed</h1>");
            document.getElementById("setMyWidth").setAttribute("style","background-color:red");
            $('#amendHTML2').css("border", "solid blue 2px");
        }
    </script>
</fieldset>

<fieldset id="setMyWidth">
    <h1>jQuery - css</h1>
    <button type="button" onclick="fnChangeText2()">Change Text</button>
    <div id="amendHTML2">hi</div>
    <script>
        function fnChangeText2() {
            $('#amendHTML2').html("<h1>I am changed</h1>");
            document.getElementById("setMyWidth").setAttribute("style","background-color:red");
            $('#amendHTML2').css("border", "solid blue 2px");
        }
    </script>
</fieldset>

<fieldset>
    <h1>Javascript - querySelector</h1>
    <button type="button" onclick="fnQuerySelector()">Change Text</button>
    <div id="querySelector">hi</div>
    <script>
        function fnQuerySelector() {
            document.querySelector('#querySelector').setAttribute("style", "background-color:green");
        }
    </script>
</fieldset>

<fieldset>
    <h1>Javascript - Global and Local Scope</h1>
    <div id="scope" onclick="fnScope()">Scope</div>
    <script>
        "use strict";
        var scopeX = 1;
        console.log(scopeX);            // GLOBAL
        function fnScope() {
            console.log(scopeX);
            var privateVar = 3;         // PRIVATE
            console.log(privateVar);
            if (privateVar === 3) {
                let t = 22;
                console.log(t);
            }
            const xx = 555;
        }
    </script>
</fieldset>

<fieldset>
    <h1>Javascript - var, let and const</h1>
    <div id="scope" onclick="fnScope()">Scope</div>
    <script>
        "use strict";
        var scopeX = 1;
        console.log(scopeX);            // GLOBAL
        function fnScope() {
            console.log(scopeX);
            var privateVar = 3;         // PRIVATE
            console.log(privateVar);
            if (privateVar === 3) {
                let t = 22;
                console.log(t);
            }
            const xx = 555;
        }
    </script>
</fieldset>

<fieldset>
    <h1>Javascript - setTimeout and setInterval</h1>
    <div id="delay" onclick="fnDelay()">Delay</div>
    <div id="timer" onclick="fnTimer()">Timer</div>
    <script>
        function fnDelay() {
            setTimeout(function () {
                document.getElementById("delay").style.backgroundColor = "blue"; //EASIER AND BETTER
                //document.getElementById("delay").setAttribute("style", "background-color:blue");                    // set DELAY DIV TO CHANGE BACKGROUND
            }, 2000);
        }
        function fnTimer() {
            setInterval(function () {
                var d = new Date();
                document.getElementById("timer").innerHTML = d.toLocaleTimeString();
            }, 1000);
        }

    </script>
</fieldset>

<fieldset>
    <h1>Javascript - web worker</h1>
    <div id="worker" onclick="fnWorker()">Web Worker</div>
    <script>
        function fnWorker() {
            var w = new Worker("assets/js/webworker.js");
            w.onmessage=function(event){
                console.log(event.data);
            }
            w.postMessage("You are my worker and you will do whatever I command you");
            
        }
    </script>
</fieldset>
```

## webworker

```js
console.log("Inside webWorker");
onmessage = function (event) {
    console.log('worker has received a message ' + event.data);
}
setTimeout(function () {
    console.log(new Date());
    postMessage('Sending message back to main page ' + new Date());
}, 1000);
```