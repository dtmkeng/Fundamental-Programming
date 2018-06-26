## Recursion
### Background
    In this way it is often possible to solve
    seemingly complex problems via repeated application of very simple solutions to the subproblems
    A recursive function is a function that calls itself somewhere in its definition, i.e., in some sense, the function is defined in terms of itself
### Flawed Recursion
    We will consider the proper implementation of a recursive function in a moment, but let’s start
    by considering some flawed implementations because it is important to recognize how you must
    not implement a recursive function  

```py
>>> def r2(n):
        2 ... print(n, "Start")
        3 ... r2(n + 1)
        4 ... print(n, "End")
        5 ...
        12.3. PROPER RECURSION 299
        6 >>> r2(0)
        7 0 Start
        8 1 Start
        9 2 Start
        10 .
        11 . <<OUTPUT DELETED>>
        12 .
        13 994 Start
        14 995 Start
        15 996 Start
        16 Traceback (most recent call last):
        17 File "<stdin>", line 1, in <module>
        18 File "<stdin>", line 3, in r2
        19 File "<stdin>", line 3, in r2
        20 .
        21 . <<OUTPUT DELETED>>
        22 .
        23 File "<stdin>", line 2, in r2
        24 RuntimeError: maximum recursion depth exceeded while calling a Python
        25 object 
```
### Proper Recursion
1. There must be a reachable base case where the function stops calling itself.
2. The argument of the function must be modified with each call.
    ```py
        1 >>> def r3(n):
        2 ... if n < 4: # General case.
        3 ... print(n, "Start")
        4 ... r3(n + 1)
        5 ... print(n, "End")
        6 ... else: # Base case.
        7 ... print(n, "Start")
        8 ... print(n, "End")
        9 ...
        10 >>> r3(0)
        11 0 Start
        12 1 Start
        13 2 Start
        14 3 Start
        15 4 Start
        16 4 End
        17 3 End
        18 2 End
        19 1 End
        20 0 End
    ```
### Merge Sort
```py
    >>> def merge(left, right):
    2 ... result = [] # Accumulator for merged list.
    3 ... while len(left) > 0 or len(right) > 0:
    4 ... if len(left) > 0 and len(right) > 0:
    5 ... if left[0] <= right[0]: # left smaller than right.
    6 ... result.append(left[0]) # Append element from left.
    7 ... left = left[1 : ] # Remove first left element
    8 ... else: # right smaller than left.
    9 ... result.append(right[0]) # Append element from right.
    10 ... right = right[1 : ] # Remove first right element.
    11 ... elif len(left) == 0: # No elements in left.
    12 ... result.extend(right) # Extend by remaining right elements.
    13 ... break # Terminate loop.
    14 ... else: # No elements in right.
    15 ... result.extend(left) # Extend by remaining left elements.
    16 ... break # Terminate loop.
    17 ... print("result: ", result) # For sake of illustration.
    18 ... return result
```
#### explame
```py
    >>> merge([1, 4], [2, 3])
    2 result: [1]
    3 result: [1, 2]
    4 result: [1, 2, 3]
    5 [1, 2, 3, 4]
    6 >>> merge([1, 5, 10], [0, 4, 6, 7, 8])
    7 result: [0]
    8 result: [0, 1]
    9 result: [0, 1, 4]
    10 result: [0, 1, 4, 5]
    11 result: [0, 1, 4, 5, 6]
    12 result: [0, 1, 4, 5, 6, 7]
    13 result: [0, 1, 4, 5, 6, 7, 8]
    14 [0, 1, 4, 5, 6, 7, 8, 10]
```