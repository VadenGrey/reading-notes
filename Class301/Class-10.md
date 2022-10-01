# Class 10

**Understanding the JavaScript Call Stack**
1. a function
2. one at a time
3. Last In, First Out
4. 

```
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();
```
5. A stack overflow occurs when there is a recursive function

**JavaScript error messages**
1. thing is not defined
2. improper syntax
3. invalid length
4. invalid type of variable accessed
5. a point where code stops running
6. serves as a breakpoint

**things I want to know more about**

references

[Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

[JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)