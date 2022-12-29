# Class 08

**List Comprehensions**

You can use methods in lists to fill out said lists like:
```python
my_new_list = [x for x in range(10)]
```
which my_new_list would look like: [1,2,3,4,5,6,7,8,9]

Lists can be made with loops as well and any function that has outputs:
```python
squares = []

for x in range(10):
    # raise x to the power of 2
    squares.append(x**2)
```
which squares will look like: [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

references

[List Comprehensions](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)


<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)