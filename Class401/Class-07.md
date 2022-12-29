# Class 07

**Python Scope**

The concept of scope rules how variables and names are looked up in your code. It determines the visibility of a variable within the code.

Global scope: The names that you define in this scope are available to all your code.

Local scope: The names that you define in this scope are only available or visible to the code within the scope.

<br>

Python resolves names using the so-called LEGB rule, which is named after the Python scope for names. The letters in LEGB stand for Local, Enclosing, Global, and Built-in.

Local (or function) scope is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function.

Enclosing (or nonlocal) scope is a special scope that only exists for nested functions.

Global (or module) scope is the top-most scope in a Python program, script, or module.

Built-in scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session.


references

[Python Scope](https://realpython.com/python-scope-legb-rule/)



<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)