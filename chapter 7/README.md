## Review Questions (page 172)
1. What output isproduced by the following code?
```py
    xlist = [1, [1, 2], [1, 2, 3]]
    print(xlist[1])
```
output : 
```py
  [1 , 2]
```

2. What output is produced by the following code?
```py
    xlist = [1, [1, 2], [1, 2, 3]]
    print(xlist[1][1])
```
output: 
```py
    2
```
3. What output is produced by the following code?
```py
    xlist = [1, [1, 2], [1, 2, 3]]
    print(xlist[1] + [1])
```
output: 
```py
    [1, 2, 1]
```
4. What output is produced by the following code?
```py
    def sum_part(xlist, n):
        sum = 0
        for x in xlist[n]:
            sum = sum + x
        return sum
    ylist = [[1, 2], [3, 4], [5, 6], [7, 8]]
    x = sum_part(ylist, 2)
    print(x)
```
output: 
```py
    11 #sum list [5, 6]
```
5. Assume xlist is a list of lists where the inner lists have two elements. The second
        element of these inner lists is a numeric value. Which of the following will sum the values 
        of the second element of the nested lists and store the result in sum?
    - [ ] (a) 
    ```py
            sum = 0
            for item in xlist:
                sum = sum + item[1]
    ```    
    - [x] (b) 
    ```py 
            sum = 0
            for one, two in xlist:
                sum = sum + two
    ```
    - [ ] (c) 
    ```py
            sum = 0
            for i in range(len(xlist)):
                sum = sum + xlist[i][1]
    ```
    - [ ] (d) All of the above.

6. What output is produced by the following code?
    ```py
        for i in range(3):
            for j in range(3):
                print(i * j, end="")
    ```
    - [ ] (a) 123246369
    - [ ] (b) 0000012302460369
    - [x] (c) 000012024
    - [ ] (d) None of the above.
7. What output is produced by the following code?
    ```py 
        s = "abc"
        for i in range(1, len(s) + 1):
            sub = ""
            for j in range(i):
                sub = s[j] + sub
            print(sub)
    ```
    - [x] (a) 
    ```       
            a
            ba
            cba
    ```
    - [ ] (b)
    ``` 
            a
            ab
            abc
    ```
    - [ ] (c) 
    ```
            a
            ab
    ```
    - [ ] (d) This code produces an error.
8. What output is produced by the following code?
    ```py
        s = "grasshopper"
        for i in range(1, len(s), 2):
            print(s[i], end="")
    ```
    - [ ] (a) gasopr
    - [ ] (b) gr
    - [x] (c) rshpe
    - [ ] (d) rshper
9. What output is produced by the following code?
    ```py
        x = [7]
        y = x
        x[0] = x[0] + 3
        y[0] = y[0] - 5
        print(x, y)
    ```
    output: 
    ```py
    [5] [5]
    ```
10. What output is produced by the following code?
    ```py
        x = [7]
        y = x
        x = [8]
        print(x, y)
    ```
    output:
    ```py
     [8] [7] 
    ```
11. What output is produced by the following code?
    ```py
        x = [1, 2, 3, 4]
        y = x
        y[2] = 0
        z = x[1 : ]
        x[1] = 9
        print(x, y, z)
    ```
    ```py
        [1,9,0,4] [1,9,0,4] [2,0,4]
    ```
12. What output is produced by the following code?
    ```py
        s = "row"
        for i in range(len(s)):
            print(s[ : i])
    ```
    - [x] (a)
    ```
        r
        ro
    ```
    - [ ] (b)
    ``` 
        r
        ro
        row
    ```
    - [ ] (c)
    ``` 
        ro
        row
    ```
    - [ ] (d) None of the above.
13. What output is produced by the following code?
    ```py
        s = "stab"
        for i in range(len(s)):
            print(s[i : 0 : -1])
    ```
    - [ ] (a) 
        s
        ts
        ats
        bats
    - [x] (b)
        t
        at
        bat
    - [ ] (c)
        s
        st
        sta
    - [ ] (d) None of the above.
14. What output is produced by the following code?
    ```py
        s = "stab"
        for i in range(len(s)):
            print(s[i : -5 : -1])
    ```
    - [x] (a) 
    ```
        s
        ts
        ats
        bats
    ```
    - [ ] (b)
    ```
        t
        at
        bat
    ```
    -  [ ] (c)
    ```
        s
        st
        sta
    ```
    - [ ] (d) None of the above.
15. What output is produced by the following code?
```py
s = "stab"
    for i in range(len(s)):
        print(s[0 : i : 1])
```
- [ ] (a) 
```
    s
    ts
    ats
    bats
```
- [ ] (b)
```
    t
    at
    bat
```
- [ ] (c)
```
    s
    st
    sta
```
- [ ] (d) None of the above.