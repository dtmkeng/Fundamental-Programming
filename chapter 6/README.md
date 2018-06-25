## REVIEW QUESTIONS (page 133)
1. True or False: The length of a list is given by the length() function.
    ans `False` it use `len(list)` 
2. True or False: The index for the first element of a list is 1, e.g., xlist[1] is the first
element of the list xlist.
    ans `False` first index of `list` is `0` 
3. What is the output produced by the following code?
    ```py
        xlist = []
        xlist.append(5)
        xlist.append(10)
        print(xlist)
    ```
    - [x] (a) [5, 10]
    - [ ] (b) []
    - [ ] (c) 5, 10
    - [ ] (d) 5 10
    - [ ] (e) This produces an error.
    - [ ] (f) None of the above.

4. What is the output produced by the following code?
    ```py
        zlist = []
        zlist.append([3, 4])
        print(zlist)
    ```
    - [ ] (a) [3, 4]
    - [x] (b) [[3, 4]]
    - [ ] (c) 3, 4
    - [ ] (d) 3 4
    - [ ] (e) None of the above.
5. What is the value of xlist2 after the following statement has been executed?
    ```py
        xlist2 = list(range(-3, 3))
    ```
    - [ ] (a) [-3, -2, -1, 0, 1, 2, 3]
    - [x] (b) [-3, -2, -1, 0, 1, 2]
    - [ ] (c) [-2, -1, 0, 1, 2]
    - [ ] (d) [-3, 0, 3]
    - [ ] (e) This produces an error.
6. What is the value of xlist3 after the following statement has been executed?
    ```py
        xlist3 = list(range(-3, 3, 3))
    ```
    - [ ] (a) [-3, 0, 3]
    - [x] (b) [-3, 0]
    - [ ] (c) [-2, 1]
    - [ ] (d) This produces an error.

7. What is the value of xlist4 after the following statement has been executed?
    ```py
        xlist4 = list(range(-3))
    ```
    - [x] (a) []
    - [ ] (b) [-3, -2, -1]
    - [ ] (c) [-3, -2, -1, 0]
    - [ ] (d) This produces an error.

8. What is output produced by the following?
    ```py
        xlist = [2, 1, 3]
        ylist = xlist.sort()
        print(xlist, ylist)
    ```
    - [ ] (a) [2, 1, 3] [1, 2, 3]
    - [ ] (b) [3, 2, 1] [3, 2, 1]
    - [ ] (c) [1, 2, 3] [2, 1, 3]
    - [X] (d) [1, 2, 3] None
    - [ ] (e) This produces an error.
    `sort is not return`

9. To what value is the variable x set by the following code?
    ```PY 
        def multiply_list(start, stop):
            product = 1
            for element in range(start, stop):
                product = product * element
                return product
        x = multiply_list(1, 4)
    ```
    - [ ] (a) 24
    - [ ] (b) 6
    - [ ] (c) 2
    - [x] (d) 1
    `the return statement is in the body of the loop`

10. Consider the following function:
    ```py
        def f1(x, y):
            print([x, y])
    ```
    True or False: This function returns a list consisting of the two parameters passed to the
    function.
    ans `False (this is a void function)` 
11. Consider the following function:
    ```py
        def f2(x, y):
            return x, y
    ```
    True or False: This function returns a list consisting of the two parameters passed to the
    function.
    ans  `False (this funtion return tuple)`
12. Consider the following function:
    ```py
        def f3(x, y):
            print(x, y)
            return [x, y]
    ```
    True or False: This function returns a list consisting of the two parameters passed to the
    function.
    ans `True`
13. Consider the following function:
    ```py
        def f4(x, y):
            return [x, y]
            print(x, y)
    ```
    True or False: This function prints a list consisting of the two parameters passed to the
    function.
    ans `False (print() statement comes after the return statement and thus will not be executed`
14. Consider the following function:
    ```py
        def f5(x, y):
            return [x, y]
            print([x, y])
    ```
    True or False: This function prints a list consisting of the two parameters passed to the
    function.
    ans `Fales`
15. What output is produced by the following code?
    ```py
        xlist = [3, 2, 1, 0]
        for item in xlist:
            print(item, end=" ")
    ```
    - [ ] (a) 3210
    - [x] (b) 3 2 1 0
    - [ ] (c) [3, 2, 1, 0]
    - [ ] (d) This produces an error.
    - [ ] (e) None of the above.
16. What output is produced by the following code?
    ```py
        a = 1
        b = 2
        xlist = [a, b, a + b]
        a = 0
        b = 0
        print(xlist)
    ```
    - [ ] (a) [a, b, a b]+
    - [x] (b) [1, 2, 3]
    - [ ] (c) [0, 0, 0]
    - [ ] (d) This produces an error.
    - [ ] (e) None of the above.
17. What output is produced by the following code?
    ```py
        xlist = [3, 5, 7]
        print(xlist[1] + xlist[3])
    ```
    - [ ] (a) 10
    - [ ] (b) 12
    - [ ] (c) 4
    - [X] (d) This produces an error.
    - [ ] (e) None of the above.
18. What output is produced by the following code?
    ```py
        xlist = ["aa", "bb", "cc"]
        for i in [2, 1, 0]:
            print(xlist[i], end=" ")
    ```
    - [ ] (a) aa bb cc
    - [x] (b) cc bb aa
    - [ ] (c) This produces an error.
    - [ ] (d) None of the above.
19. What does the following code do?
    ```py
        for i in range(1, 10, 2):
            print(i)
    ```
    - [x] (a) Prints all odd numbers in the range [1, 9].
    - [ ] (b) Prints all numbers in the range [1, 9].
    - [ ] (c) Prints all even numbers in the range [1, 10].
    - [ ] (d) This produces an error.
20. What is the result of evaluating the expression `list(range(5))`?
    - [x] (a) [0, 1, 2, 3, 4]
    - [ ] (b) [1, 2, 3, 4, 5]
    - [ ] (c) [0, 1, 2, 3, 4, 5]
    - [ ] (d) None of the above.
21. Which of the following headers is appropriate for implementing a counted loop that executes
4 times?
    - [ ] (a) `for i in 4:`
    - [ ] (b) `for i in range(5):`
    - [x] (c) `for i in range(4):`
    - [ ] (d) `for i in range(1, 4):`
22. Consider the following program:
```py
    def main():
        num = eval(input("Enter a number: "))
        for i in range(3):
            num = num * 2
        print(num)
    main()
```
    Suppose the input to this program is 2, what is the output?
- [ ] (a) 2
          4
          8
- [ ] (b) 4
          8
- [ ] (c) 4
          8
         16
- [x] (d)16

23. The following fragment of code is in a program. What output does it produce?
    ```py 
        fact = 1
        for factor in range(4):
            fact = fact * factor
        print(fact)
    ```
    - [ ] (a) 120
    - [ ] (b) 24
    - [ ] (c) 6
    - [x] (d) 0
24. What is the output from the following program if the user enters 5.
    ```py
        def main():
            n = eval(input("Enter an integer: "))
            ans = 0
            for x in range(1, n):
                ans = ans + x
            print(ans)
        main()
    ```
    - [ ] (a) 120
    - [x] (b) 10
    - [ ] (c) 15
    - [ ] (d) None of the above.
25. What is the output from the following code?
    ```py
    s = ['s', 'c', 'o', 'r', 'e']
    for i in range(len(s) - 1, -1, -1):
        print(s[i], end = " ")
    ```
    - [ ] (a) s c o r e
    - [x] (b) e r o c s
    - [ ] (c) 4 3 2 1 0
    - [ ] (d) None of the above.
26. The following fragment of code is in a program. What output does it produce?
    ```py
        s = ['s', 'c', 'o', 'r', 'e']
        sum = 0
        for i in range(len(s)):
            sum = sum + s[i]
        print(sum)
    ```
    - [ ] (a) score
    - [ ] (b) erocs
    - [ ] (c) scor
    - [ ] (d) 01234
    - [x] (e) None of the above.
27. The following fragment of code is in a program. What output does it produce?
    ```py
        s = ['s', 'c', 'o', 'r', 'e']
        sum = ""
        for i in range(len(s)):
            sum = s[i] + sum
        print(sum)
    ```
    - [ ] (a) score
    - [x] (b) erocs
    - [ ] (c) scor
    - [ ] (d) 01234
    - [ ] (e) None of the above.
28. What is the value returned by the following function when it is called with an argument of 3
    (i.e., summer1(3))?
    ```py 
        def summer1(n):
            sum = 0
            for i in range(1, n + 1):
                sum = sum + i
            return sum
    ```
    - [ ] (a) 3
    - [x] (b) 1
    - [ ] (c) 6
    - [ ] (d) 0
29. What is the value returned by the following function when it is called with an argument of 4
    (i.e., summer2(4))?
    ```py
        def summer2(n):
            sum = 0
            for i in range(n):
                sum = sum + i
            return sum
    ```
    - [x] (a) 3
    - [ ] (b) 1
    - [ ] (c) 6
    - [ ] (d) 0
30. Consider the following function:
    ```py
        def foo():
            xlist = []
            for i in range(4):
                x = input("Enter a number: ")
                xlist.append(x)
            return xlist
    ```
        Which of the following best describes what this function does?
    - [ ] (a) It returns a list of four numbers that the user provides.
    - [x] (b) It returns a list of four strings that the user provides.
    - [ ] (c) It returns a list of three numbers that the user provides.
    - [ ] (d) It produces an erro