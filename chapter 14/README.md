# Dictionaries
### define Dictionaries 
```py
   dic = {'name': 'Funda','age':12}
   print(dic['name']) 
   # output 
   Funda
```
### for-loop, the loop variable takes on the values of key
```py 
    1 >>> abe = {’name’ : ’Abraham Lincoln’, ’age’ : 203, ’height’ : 193}
    2 >>> for foo in abe:
    3 ... print(foo)
    4 ...
    5 age
    6 name
    7 height
    8 >>> for foo in abe.keys():
    9 ... print(foo)
    10 ...
    11 age
    12 name
    13 height 
```
### items() method to obtain both the key and the associated value in the header of the for-loop
```py
    1 >>> abe = {'nam' : 'Abraham Lincoln', 'age' : 203, 'height' : 193}
    2 >>> for key, value in abe.items()
    3 ... print(key, ':\t', value, sep="")
    4 ...
    5 age: 203
    6 name: Abraham LincolnS
    7 height: 193

```
### Displaying the values in a dictionary.
```py
    1 >>> abe = {'name' : 'Abraham Lincoln', 'age' : 203, 'height' : 193}
    2 >>> for value in abe.values():
    3 ... print(value)
    4 ...
    6 Abraham Lincoln
    7 193 
```
### Use of sorted() to `sort the keys` of a dict and thus show the data “in order.”
```py
        1 >>> students = {
        2 ... 'Harry' : 'B+', 'Hermione' : 'A+', 'Ron' : 'B-',
        3 ... 'Fred' : 'C', 'George':'C', 'Nevel' : 'B',
        4 ... 'Lord Voldemort' : 'F', 'Ginny' : 'A'
        5 ... }
        6 >>> for key in sorted(students): # Sorted keys.
        7 ... print("{:2} {}".format(students[key], key))
        8 ...
        9 C Fred
        10 C George
        11 A Ginny
        12 B+ Harry
        13 A+ Hermione
        14 F Lord Voldemort
        15 B Nevel
        16 B- Ron
        17 >>> for key in students: # Unsorted keys.
        18 ... print(students[key], key)
        19 ...
        14.3. GET() 341
        20 A+ Hermione
        21 B- Ron
        22 B+ Harry
        23 B Nevel
        24 F Lord Voldemort
        25 A Ginny
        26 C George
        27 C Fred
```
### The get() method can be used to look up values for a given key. If the key does not exist, the method returns None.
```py
    1 >>> james = {'age': 261, 'height': 163}
    2 >>> for key in ['name','age', 'height']:
    3 ... print(key, ':\t', james.get(key), sep="")
    4 ...
    5 name: None
    6 age: 261
    7 height: 163
    8 >>> for key in ['name', 'age', 'height']:
    9 ... print(key, ':\t', james[key], sep="")
    10 ...
    11 Traceback (most recent call last):
    12 File "<stdin>", line 2, in <module>
    13 KeyError: ’name’
```
## Review Questions (page 344)
1. What is the output produced by the following code?
    ```py
        d = {'a' : 0, 'b': 1, 'c' : 2}
        print(d['c'])
    ```
    - [ ] (a) c
    - [x] (b) 2
    - [ ] (c) `'c' : 2`
    - [ ] (d) This code produces an error.

2. What is the output produced by the following code?
    ```py
        d = {'a' : 0, 'b': 1, 'c' : 2}
        print(d[2])
    ```
    - [ ] (a) c
    - [ ] (b) 2
    - [ ] (c) `'c' : 2` 
    - [x] (d) This code produces an error.

3. What is the output produced by the following code?
    ```py
        d = {'a' : 0, 'b': 1, 'c' : 2}
        print(d.get(2, 'c'))
    ```
    - [x] (a) c
    - [ ] (b) 2
    - [ ] (c) `'c' : 2`
    - [ ] (d) This code produces an error.
4. What is the output produced by the following code?
    ```py
        d = {'a' : 0, 'b': 1, 'c' : 2}
        for x in sorted(d):
            print(d[x], end=" ")
    ```
    - [ ] (a) a b c
    - [x] (b) 0 1 2
    - [ ] (c) ('a', 0) ('b', 1) ('c', 2)
    - [ ] (d) This code produces an error.
5. What is the output produced by the following code?
    ```py   
        d = {'a' : 0, 'b': 1, 'c' : 2}
        for x in sorted(d.values()):
            print(x, end=" ")
    ```
    - [ ] (a) a b c
    - [x] (b) 0 1 2
    - [ ] (c) ('a', 0) ('b', 1) ('c', 2)
    - [ ] (d) This code produces an error.
6. What is the output produced by the following code?
    ```py
        d = {'a' : 0, 'b': 1, 'c' : 2}
        for x in sorted(d.items()):
            print(x, end=" ")
    ```
    - [ ] (a) a b c
    - [ ] (b) 0 1 2
    - [x] (c) (’a’, 0) (’b’, 1) (’c’, 2)
    - [ ] (d) This code produces an error.
7. What is the output produced by the following code?
    ```py
        d = {'a' : 0, 'b': 1, 'c' : 2}
        for x in sorted(d.keys()):
            print(x, end=" ")
    ```
    - [x] (a) a b c
    - [ ] (b) 0 1 2
    - [ ] (c) ('a', 0) ('b', 1) ('c', 2)
    - [ ] (d) This code produces an error.

8. What is the output produced by the following code?
    ```py
        pres = {'george' : 'washington', 'thomas' : 'jefferson', 'john' : 'adams'}
        print(pres.get('washington', 'dc'))
    ```
    - [ ] (a) george
    - [ ] (b) washington
    - [x] (c) dc
    - [ ] (d) This code produces an error.
9. What is the output produced by the following code?
    ```py
    pres = {'george' : 'washington', 'thomas' : 'jefferson', 'john' : 'adams'}
    for p in sorted(pres):
        print(p, end=" ")
    ```
    - [ ] (a) george thomas john
    - [x] (b) george john thomas
    - [ ] (c) washington jefferson adams
    - [ ] (d) adams jefferson washington
    - [ ] (e) None of the above.

