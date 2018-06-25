# Review Questions (page 43)
1. What does Python print as a result of this statement:
   `print(7 + 23)`
   - [ ] 7 + 23
   - [ ] 7 + 23 = 30
   - [x] 30
   - [ ] This produces an error.
    running 
    ```
    >>> print(7 + 23)
    30
    ```
2. Which of the following are valid variable names?
    - [x] _1_2_3_
    - [ ] ms.NET
    - [x] WoW
    - [ ] green-day
    - [ ] big!fish
    - [ ] 500_days_of_summer

3. Which of the following are valid identifiers?
    - [x] a1b2c
    - [x] 1a2b3
    - [x] a_b_c
    - [ ] _a_b_
    - [ ] a-b-c
    - [ ] -a-b- 
    - [x] aBcDe
    - [ ] a.b.c
    example
    ```
        one2three   Valid.
        one 2 three Valid.
        1 2 three   Invalid. Cannot start with a digit. 
        one-2-three Invalid. Cannot have hyphens (minus signs).
        n31         Valid.
        n.31        Invalid. Cannot have periods.
        trailing    Valid.
        leading     Valid.
        net worth   Invalid. Cannot have blank spaces.
        vArIaBlE    Valid
    ``` 
4. Suppose the variable x has the value 5 and y has the value 10. After executing these statements:
    ```
        x = y
        y = x
    ```
    what will the values of x and y be, respectively?
    - [ ] 5 and 10
    - [ ] 10 and 5
    - [x] 10 and 10
    - [ ] 5 and 5

5. True or False: “x ** 2” yields the identical result that is produced by “x * x” for all
integer and float values of x.
`True`
6. True or False: “x ** 2.0” yields the identical result that is produced by “x * x” for all
integer and float values of x.
`False`
7. What does Python print as a result of this statement?
    `print(5 + 6 % 7)`
    - [ ] This produces an error.
    - [ ] 5 + 6 % 7
    - [x] 11
    - [ ] 4
8. What is the output from the print() statement in the following code?
    ```
    x = 3 % 4 + 1
    y = 4 % 3 + 1
    x, y = x, y
    ```
    `print(x, y)`
    - [ ] 2 4
    - [x] 4 2
    - [ ] 0 3
    - [ ] 3 0
9. What is the output produced by the following code?
    ```
    x = 3
    y = 4
    print("x", "y", x + y)
    ```
    - [ ] 3 4 7
    - [x] x y 7
    - [ ] x y x + y
    - [ ] 3 4 x + y
    - [ ] x y 34

For each of the following, determine the value to which the expression evaluates. (Your answer
should distinguish between floats and ints by either the inclusion or exclusion of a decimal point.)
10. 5.5 - 11 / 2
ans `0.0`
11. 5.5 - 11 // 2
ans `0.5`
12. 10 % 7
ans `3`
13. ` 7  % 10`
ans `7`
14. 3 + 2 * 2
ans `7`
15. 16 / 4 / 2
ans `2.0`
16. 16 / 4 * 2 
ans `8.0`

17. Given that the following Python statements are executed:
    ```
        a = 2
        b = a + 1 // 2
        c = a + 1.0 // 2
        d = (a + 1) // 2
        e = (a + 1.0) // 2
        f = a + 1 / 2
        g = (a + 1) / 2
    ```
    - Ans
    ```
    b = 2
    c = 2.0 
    d = 1 
    e = 1.0
    f = 2.5
    g = 1.5 
    ```
    `Determine the values to which the variables b through g are set.`

18. What output is produced when the following code is executed?
    ```
        hello = "yo"
        world = "dude"
        print(hello, world)
    ```
    - [ ] hello, world
    - [x] yo dude
    - [ ] "yo" "dude"
    - [ ] yodude
    - [ ] This produces an error.
19. The following code is executed. What is the output from the print() statement?
    ```
        x = 15
        y = x
        x = 20
        print(y)
    ``` 
    - [x] 15
    - [ ] 20
    - [ ] y
    - [ ] x
    - [ ] This produces an error.

20. The following code is executed. What is the output from the print() statement?
    ```
        result = "10" / 2
        print(result)
    ```
    - [ ] 5
    - [ ] 5.0
    - [ ] '"10" / 2'
    - [X] This produces an error.

21. The following code is executed. What is the output from the print() statement?
    ```
    x = 10  
    y = 20
    a, b = x + 1, y + 2
    print(a, b)
    ```
    - [ ] 10 20
    - [ ] 11 22
    - [ ] 'a, b'
    - [ ] 'x + 1, y + 2'
    - [ ] This produces an error.
22. True or False: In general, “x / y * z” is equal to “x / (y * z)”.
    ans `False`
23. True or False: In general, “x / y ** z” is equal to “x / (y ** z)”.
    ans `True`
24. True or False: In general, “w + x * y + z” is equal to “(w + x) * (y + z)”.
    ans `False`
25. True or False: In general, “w % x + y % z” is equal to “(w % x) + (y % z)”.
    ans `True`
26. True or False: If both m and n are ints, then “m / n” and “m // n” both evaluate to
ints.
    ans `False`
27. True or False: The following three statements are all equivalent:
```
x = (3 +
4)
x = 3 + \
4
x = """3 +
4"""
```
ans `False`

28. Given that the following Python statements are executed:
    ```
        x = 3 % 4
        y = 4 % 3
    ```
    What are the values of x and y?
    ```
    x = 3 
    y = 1 
    ```
29. To what value is the variable z set by the following code?
    `z = 13 + 13 // 10`
    - [ ] 14.3
    - [ ] 14.0
    - [ ] 2
    - [x] 14
    - [ ] 16
30. Assume the float variable ss represents a time in terms of seconds. What is an appropriate
statement to calculate the number of complete minutes in this time (and store the result as an
int in the variable mm)?
    - [x] mm = ss // 60
    - [ ] mm = ss / 60
    - [ ] mm = ss % 60
    - [ ] mm = ss * 60
31. To what values does the following statement set the variables x and y?
    `x, y = divmod(13, 7)`
    - [ ] 6 and 1
    - [x] 1 and 6
    - [ ] 6.0 and 2.0
    - [ ] This produces an error.
    ``` divmode(a,b) == a // b , a % b ```
