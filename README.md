# learning-javascript
Short notes on JavaScript for reference (all taken from http://javascript.info)

F12 for console

server-side: "node my.js"<br>
browser: <script></script>

<script src="/path/to/script.js"></script> absolute from root<br>
<script src="script.js"></script> relative from current page

short: inside script tag<br>
long: external file for cache/speed

separate statements with ;

use comments to describe what happens and why or to disable code<br>
one-line comments // comment here (shortcut Ctrl+/)<br>
multiline comments /* comment here */ (shortcut Ctrl+Shift+/)

!!!IMPORTANT!!!<br>
always start with<br>
'use strict';<br>
at the top

Variable is a named box for data. We can put any value into the box. We can change the value as many times as needed. When the value is changed, old data is replaced with new data (side note: functional programming languages like Scala or Erland can't change variable value once stored).

Example<br>
let message; // this created a variable called message<br>
let name; // this created a variable called name<br>
message = 'Hello'; // value is Hello<br>
message = 'Hi'; // value is now Hi<br>
name = 'World';<br>
message = name; // value is now World<br>
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

Example<br>
const COLOR_RED = "#F00";<br>
const COLOR_ORANGE = "#FF7F00";<br>
const pageLoadTime = /* time taken by a webpage to load */;<br>
let color;<br>
color = COLOR_ORANGE;<br>
alert(color); // #FF7F00

JavaScript is "dynamically typed"<br>
Dynamically typed is when a variable is not bound to any specific data type<br>
There are 7 basic data types

1) number - integer, floating point numbers, Infinity, -Infinity, NaN (error, sticky meaning if a part is NaN, the whole result is NaN)
2) string - must be quoted, double quotes, single quotes, backticks (you can embed variables and expressions into string)<br>
Example<br>
let name = "John";<br>
alert( `Hello, ${name}!` ); // embed variable... Hello, John!<br>
alert( `the result is ${1 + 2}` ); // embed expression... the result is 3
3) boolean - true, false, can come as result of comparisons
4) "null" value - nothing, empty value, use null to set variable value to empty
5) "undefined" value - value not assigned, only used for checks to see if the variable is assigned
6) objects (not primitive like the rest, stores collections of data) and symbols (unique identifiers for objects)
7) typeof - returns data type, useful when we want to process values of different types differently or for quick checking<br>
supports two forms of syntax<br>as an operator: typeof x<br>function style: typeof(x)

Type Conversion - operators and functions automatically convert a value to the right type

But sometimes we will need to explicitly convert a value manually to put things right
- String conversion: String(value);
- Number conversion: Number(value);
  - undefined becomes... NaN
  - null becomes... 0
  - true and false becomes... 1 and 0
  - string becomes... whitespaces from start/end are removed, then if remaining string is empty... result is 0 and error is NaN
  - alert ( 1 + '2' ); // addition '+' concatenates strings so result would be '12' string type
- Boolean conversion: Boolean(value);
  - values that are 0, empty string, null, undefined, NaN become false (except for string "0" and " " which is true)
  - other values become true

Operators is addition, multiplication, subtraction, etc<br>
Operators runs from left to right and addition '+' concatenates and converts into string<br>
Example<br>
alert (2 + 2 + '1'); // "41"<br>
Operand or arguments is what operators are applied to (5 x 2... left operand is 5 and right operand is 2)<br>
Unary if it has single operand<br>
Binary if it has two operands
  
  
  

























