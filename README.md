# learning-javascript
Short notes on JavaScript for reference (all taken from http://javascript.info)

F12 for console

server-side: "node my.js"<br>
browser: <script></script>

<script src="/path/to/script.js"></script> absolute from root<br>
<script src="script.js"></script> relative from current page

short: inside script tag<br>
long: external file<br>
for cache/speed

separate statements with ;

use comments to describe what happens and why or to disable code<br>
one-line comments // comment here (shortcut Ctrl+/)<br>
multiline comments /* comment here */ (shortcut Ctrl+Shift+/)

!!!IMPORTANT!!!<br>
always start with<br>
'use strict';<br>
at the top

Variable is a named box for data. We can put any value into the box. We can change the value as many times as needed. When the value is changed, old data is replaced with new data (side note: functional programming languages like Scala or Erland can't change variable value once stored).

Example
let message; // this created a variable called message
let name; // this created a variable called name
message = 'Hello'; // value is Hello
message = 'Hi'; // value is now Hi
name = 'World';
message = name; // value is now World
alert(message); // should display 'World'

Variable names
- must contain only letters, digits, symbols $ and _
- must not start with a digit
- recommend use of camelCase if multiple words
- case matters... variables named apple and AppLE are two different variables
- can't use reserved words: let, class, return, function
- use good descriptive-and-concise names (first time readers can understand what is being stored)

Constant variables
- once value is stored, it can't be changed
- use UPPERCASE and underscores for hard-coded values like hexadecimals and pi
const COLOR_RED = "#F00";
const COLOR_ORANGE = "#FF7F00";
const pageLoadTime = /* time taken by a webpage to load */;
let color;
color = COLOR_ORANGE;
alert(color); // #FF7F00
