# Programming with JavaScript

**Control Flow**

The order at which statements are executed is called control flow

A typical script in JavaScript includes many control structures, including conditionals, loops and functions. Parts of a script may also be set to execute when events occur.

## Functions

A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses (). The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)

 The code to be executed, by the function, is placed inside curly brackets: {}

 Function structure:
 ```
 function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
 ```

The code inside a function will execute when "something" **invokes** (calls) the function:
- When an event occurs (when a user clicks a button)
- When it is invoked (called) from JavaScript code
- Automatically (self invoked)

Functions often compute a return value. The return value is "returned" back to the "caller":

```
let x = myFunction(4, 3);   // Function is called, return value will end up in x

function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
}
```

You can define a function once and reuse it as much as you like!

Say if you had:
```
const input = prompt("yes or no?")
```
The script would immediatly prompt the user "yes or no?"

But if you wanted that prompt to open only when you wanted a button pressed you would write:
```
const element = document.getElementById("button");
if(element){
    element.addEventListener('click', buttonclick, false);
  }


function buttonclick() {
    let input = prompt("Enter Giveaway!? y/n")
    console.log(input)
    
    if (input == "y") {
        window.open("https://www.youtube.com/watch?v=tS_2hEmGnzA&ab_channel=Adroon");
    
    } else if (input == "n") {
        window.open("https://www.youtube.com/watch?v=dQw4w9WgXcQ&ab_channel=RickAstley");
    }

} 

```
You can use functions as variables aswell:
```
//Instead of using a variable to store the return value of a function:

let x = toCelsius(77);
let text = "The temperature is " + x + " Celsius";

//You can use the function directly, as a variable value:

let text = "The temperature is " + toCelsius(77) + " Celsius";
```




## Operators
**Basic Operators**

The assignment operator (=) assigns a value to a variable.
The addition operator (+) adds numbers:
The multiplication operator (*) multiplies numbers.

**Aritmetic Operators**
```
+	Addition
-	Subtraction
*	Multiplication
**	Exponentiation (ES2016)
/	Division
%	Modulus (Division Remainder)
++	Increment
--	Decrement
```

**Assignment Operators**
Operator	Example 	Same As
```
=	        x = y	    x = y
+=	        x += y	    x = x + y
-=	        x -= y	    x = x - y
*=	        x *= y	    x = x * y
/=	        x /= y	    x = x / y
%=	        x %= y	    x = x % y
**=	        x **= y	    x = x ** y

```


**Concantenation**

Example:
```
let text1 = "What a very ";
text1 += "nice day";
```
The result of text1 will be:

What a very nice day










References:

[W3schools Functions](https://www.w3schools.com/js/js_functions.asp) <br>
[W3schools Operators](https://www.w3schools.com/js/js_operators.asp)



[Back to main page](https://vadengrey.github.io/reading-notes/)
