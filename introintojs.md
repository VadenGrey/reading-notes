# Intro into JavaScript

Java and JavaScript are not the same!

JavaScript is a prototype-based, multi-paradigm, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles

One of its uses is that it makes websites interactable and do things

**JavaScript is declarative language, 4 ways to declare a variable**:
```
var
let
const
```
Or just by using nothing

So what are variables?

**Variables** are containers for storing data (storing data values)
```
var x = 5;
var y = 6;
var z = x + y;
```

var is an older variable(1995-2015) and you should use let and const

**When to use let and const**:

if you want a rule that cannot change use const
if you think the value of the variable can change, use let
In the example, price1, prace2, and total, are variables
```
const price1 = 5;
const price2 = 6;
let total = price1 + price2;
```
**Like algebra variables hold values which can also be used in expressions**:
```
let x = 5;
let y = 6;
let z = x + y;
```
**All JS variables must be identified with unique names**
these unique names are called ***identifiers*** (x, y, z) and they are case sensitive

The equal sign(=) in JavaScript is an "assignment" operator not an "equals sign" and a way this differs from algebra is like so:
```
x = x + 5
```
It calculates the value of x + 5 and puts the result into x. The value of x is incremented by 5.

The actual equals operator is "=="

**Datatypes**
Variables can hole values like 100 and "john doe", while text values are called text strings. Strings are written inside double or single quotes with numbers are written without if you put a number in quotes it will be treated as a text string.

**Declaring and Assigning**
Its good programming practice to declare all variables at the beginning of the script.
Example of declaring a variable and assigning a value to it:
```
let  carName = "Challenger"
```
Example of output within html:
```
<p id="demo"></p>

<script>
let carName = "Volvo";
document.getElementById("demo").innerHTML = carName;
</script>
```
You can declare many variables within one statement:
```
let person = "John Doe", carName = "Challenger", price = 60000;
```
**Concantenation**
```
let x = 2 + 3 + "5"
```
this will output 55








**Resources**:

[MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript) <br>
[Input and Output](https://code-maven.com/input-output-in-plain-javascript) 
