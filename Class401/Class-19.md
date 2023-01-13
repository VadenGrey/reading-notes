# Class 19

**Python Regular Expressions Tutorial**

Regular expressions can be used in python by firstly importing Re, and having the documentation open constantly [Regex](https://docs.python.org/3/library/re.html)

**shutil**

The shutil module includes high-level file operations such as copying and archiving.

copyfile() copies the contents of the source to the destination and raises IOError if it does not have permission to write to the destination file.
```python
# shutil_copyfile.py
import glob
import shutil

print('BEFORE:', glob.glob('shutil_copyfile.*'))

shutil.copyfile('shutil_copyfile.py', 'shutil_copyfile.py.copy')

print('AFTER:', glob.glob('shutil_copyfile.*'))
```





references

[Python Regular Expressions Tutorial](https://www.datacamp.com/tutorial/python-regular-expression-tutorial)

[shutil](https://pymotw.com/3/shutil/)

[Automation Ideas](https://www.youtube.com/watch?v=qbW6FRbaSl0&t=69s&ab_channel=Hallden)


<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)