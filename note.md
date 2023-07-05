# 1.5 Control
## Difference between if_statement and if_function
    According to condition, if_statement will choose which suites/function to call while if_function can just choose which value to return. The two function as parameters of if_function will both be called whatever the condition is true or false. 
demo:
``` python
def if_(c, t, f):
    if c:
        t
    else:
        f

from math import sqrt

def real_sqrt(x):
    """
    Return the real part of the square root of x.
    >>> real_sqrt(4)
    2.0
    >>> real_sqrt(-4)
    0.0
    """
    if x > 0:
        return sqrt(x)
    else:
        return 0.0
    """
    if_(x > 0, sqrt(x), 0.0)
    >>> real_sqrt(4)
    2.0
    >>> real_sqrt(-4)
    math domain error
    """ 
```