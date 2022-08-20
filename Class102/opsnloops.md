# Operators and loops

## Operators

**Assignment operators**
An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = f() is an assignment expression that assigns the value of f() to x.


## Loops

Here are some loops:
```
// while loops

let x = 0;
while (x <10) {
  console.log(x);
  x++
}

console.log("Out of loop")


let myFavcolor = "red";

let response;
while (response !== myFavcolor){
  response = (prompt("whats my favorite color")).toLowerCase()
  if (response !== myFavcolor) {
    alert("wrong!")
  }
}


// for loops

//     initial    condition    increment
for (let i = 0; i < 10; i = i + 2){
  console.log(i)
}

let ticketsToBuy = 40;
for (let i = 0; i <= ticketsToBuy; i += 2) {
  console.log("I bought " + i + " tickets")
}



//writing html with js
function writeIt(){
  let message = "<p>hello!</p>"
  document.write(message;)
  
}
```

**References**

[MDN Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators) <br>
[MDN Loops and iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration) <br>
[W3schools](https://www.w3schools.com/js/js_loop_for.asp)

[Back to main page](https://vadengrey.github.io/reading-notes/)


