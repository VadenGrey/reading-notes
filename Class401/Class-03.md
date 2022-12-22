# FileIO & Exceptions



**Read & Write Files in Python**

To work with a file firstly you have to open it with the function open() and its very important to close the file you have been working on with .close() as leaving the file open can cause unwanted behavior. An automatic way of closing a file is to use a with statement.
You can read files with the .read() function and write to files with the .write() function.

**Exceptions in Python**

An exception error is when syntactically correct code results in an error such like dividing by 0. You can use this to throw an exception if a certain condition is met in a script such as:

```python
x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))
```

This would result in:

Traceback (most recent call last):
  File "<\input>", line 4, in <module>
Exception: x should not exceed 5. The value of x was: 10

An Assertion error is when a condition is not met that has been asserted. Example:

```python
import sys
assert ('linux' in sys.platform), "This code runs on Linux only."
```

Output:

Traceback (most recent call last):
  File "<\input>", line 2, in <module>
AssertionError: This code runs on Linux only.


references

[Read & Write Files in Python](https://realpython.com/read-write-files-python/)

[If name equals main](https://realpython.com/python-exceptions/)

[Read & Write Files in Python](https://realpython.com/courses/reading-and-writing-files-python/)

<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)