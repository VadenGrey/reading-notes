# Class 12

**Pandas in 10**
to start:
```python
import numpy as np
import pandas as pd
```
Creating a Series by passing a list of values, letting pandas create a default integer index:
```python
s = pd.Series([1, 3, 5, np.nan, 6, 8])

s
# output:
0    1.0
1    3.0
2    5.0
3    NaN
4    6.0
5    8.0
dtype: float64
```
Creating a DataFrame by passing a NumPy array, with a datetime index using date_range() and labeled columns:
```python
dates = pd.date_range("20130101", periods=6)

dates
Out[6]: 
DatetimeIndex(['2013-01-01', '2013-01-02', '2013-01-03', '2013-01-04',
               '2013-01-05', '2013-01-06'],
              dtype='datetime64[ns]', freq='D')

df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list("ABCD"))

df
Out[8]: 
                   A         B         C         D
2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
2013-01-02  1.212112 -0.173215  0.119209 -1.044236
2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
2013-01-04  0.721555 -0.706771 -1.039575  0.271860
2013-01-05 -0.424972  0.567020  0.276232 -1.087401
2013-01-06 -0.673690  0.113648 -1.478427  0.524988
```

**What is Pandas**
Pandas is a python library that gives to a set of tools to do data analysis, in other words if your going to use python for data you're going to use pandas

With panda you can load, prepare, manipulate, model, and analyze data and it all revolves around a structure called a dataframe

references

[Pandas in 10](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

[What is Pandas](https://www.youtube.com/watch?v=dcqPhpY7tWk&t=391s&ab_channel=PythonProgrammer)

<br>

[Back to main page](https://vadengrey.github.io/reading-notes/)