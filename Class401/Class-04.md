# Class 04

**Classes and Objects**

Objects get their variables and functions from classes.

Accessing object variables:
```python
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

print(myobjectx.variable)
```

**Thinking Recursively**

Recursive functions call upon themselves until a condition has been met similar to a while loop.

Example of a recursive function that finds the factorial of a number:
```python
def factorial_recursive(n):
    # Base case: 1! = 1
    if n == 1:
        return 1

    # Recursive case: n! = n * (n-1)!
    else:
        return n * factorial_recursive(n-1)
```

**Pytest Fixtures and Coverage**

In pytest, you define fixtures using a combination of the pytest.fixture decorator, along with a function definition. For example, say you have a file that returns a list of lines from a file, in which each line is reversed:

```python
def reverse_lines(f):
   return [one_line.rstrip()[::-1] + '\n'
           for one_line in f]

```

To have more coverage on what your functions are doing, have the testing function raise an exception when it receives an unexpected output.


references

[Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

[Thinking Recursively](https://realpython.com/python-thinking-recursively/)

[Pytest Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)