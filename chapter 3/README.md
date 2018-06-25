## Review Questions (page 59)
1. The following code is executed
    `x = input("Enter x: ")`
    In response to the prompt the user enters
    `-2 * 3 + 5` 
    What is the resulting value of x?   
    - [ ] -16
    - [ ] -1
    - [x] '-2 * 3 + 5'
    - [ ] This produces an error.
2. The following code is executed
    `y = int(input("Enter x: ")) + 1` 
    In response to the prompt the user enters
    `50`
    What is the resulting value of y?
    - [ ] '50 + 1'
    - [x] 51
    - [ ] 50
    - [ ] This produces an error.
3. The following code is executed
    `y = int(input("Enter x: ") + 1)`
    In response to the prompt the user enters
    `50`
    What is the resulting value of y?
    - [ ] '50 + 1'
    - [ ] 51
    - [ ] 50
    - [x] This produces an error.
4. The following code is executed
    ```
     x = input("Enter x: ")
     print("x =", x)
    ```
    In response to the prompt the user enters
    `2 + 3 * -4`
    What is the output produced by the print() statement?
    - [ ] x = -10
    - [ ] x = -20
    - [x] x = 2 + 3 * -4
    - [ ] This produces an error.
    - [ ] None of the above.
5. The following code is executed
    ```
        x = int(input("Enter x: ")) 
        print("x =", x)
    ```
    In response to the prompt the user enters
    `2 + 3 * -4`
    What is the output produced by the print() statement?   
    - [ ] x = -10
    - [ ] x = -20
    - [ ] x = 2 + 3 * -4
    - [x] This produces an error.
    - [ ] None of the above.
6. The following code is executed
    ```
        x = int(input("Enter x: "))
        print("x =", x)
    ```
    In response to the prompt the user enters   `5.0`
    What is the output produced by the `print()` statement?       
    - [ ] x = 5.0
    - [ ] x = 5
    - [x] This produces an error.
    - [ ] None of the above.
    ```
    Traceback (most recent call last):
    File "<stdin>", line 1, in <module>
    ValueError: invalid literal for int() with base 10: '5.0'
    ```
7. The following code is executed
    ```
    x = float(input("Enter x: "))
    print("x =", x)
    ```
    In response to the prompt the user enters `5`
    What is the output produced by the `print()` statement?
    - [x] x = 5.0
    - [ ] x = 5
    - [ ] This produces an error.
    - [ ] None of the above.
8. The following code is executed
    ```
    x = eval(input("Enter x: "))
    print("x =", x)
    ```
    In response to the prompt the user enters `5`
    What is the output produced by the `print()` statement?
    - [ ] x = 5.0
    - [x] x = 5
    - [ ] This produces an error.
    - [ ] None of the above.

9. The following code is executed
    ```
    x = input("Enter x: ")
    print("x =", x)
    ```
    In response to the prompt the user enters `5`
    What is the output produced by the `print()` statement?
    - [ ] x = 5.0
    - [x] x = 5
    - [ ] This produces an error.
    - [ ] None of the above.

10. The following code is executed
    ```
    x = int(input("Enter x: "))
    print("x =", x + 1.0)
    ```
    In response to the prompt the user enters `5`
    What is the output produced by the `print()` statement?
    - [x] x = 6.0
    - [ ] x = 6 
    - [ ] This produces an error.
    - [ ] None of the above.
11. The following code is executed
    ```
    x = float(input("Enter x: "))
    print("x =", x + 1)
    ```
    In response to the prompt the user enters `5`   
    What is the output produced by the `print()` statement?
    - [x] x = 6.0
    - [ ] x = 6
    - [ ] This produces an error.
    - [ ] None of the above.

12. The following code is executed
    ```
        x = eval(input("Enter x: "))
        print("x =", x + 1)
    ```
    In response to the prompt the user enters `5`
    What is the output produced by the `print()` statement?
    - [ ] x = 6.0
    - [x] x = 6
    - [ ] This produces an error.
    - [ ] None of the above.

13. The following code is executed
    ```
    x = input("Enter x: ")
    print("x =", x + 1)
    ```
    In response to the prompt the user enters `5`
    What is the output produced by the `print()` statement?
    - [ ] x = 6.0
    - [ ] x = 6
    - [x] This produces an error.
    - [ ] None of the above.
14. The following code is executed
    ```
    x = eval(input("Enter x: "))
    print("x =", x)
    ```
    In response to the prompt the user enters `2 + 3 * -4`
    What is the output produced by the `print()` statement?
    - [x] x = -10
    - [ ] x = -20
    - [ ] x = 2 + 3 * -4
    - [ ] This produces an error.
    - [ ] None of the above.
15. What is produced by the print() statement in the following code?
    ```
    s = "8 / 4 + 4"
    print(s, eval(s), sep=" = ")
    ```
    What is the resulting value of `y` ?
    - [ ] This produces an error.
    - [ ] 8 / 4 + 4 = 6
    - [ ] 6.0 = 6.0
    - [x] 8 / 4 + 4 = 6.0
    - [ ] None of the above.
## EXERCISES 65
16. True or False: All of the following are acceptable arguments for the `int()` function: 5,
5.0, "5", and "5.0" (these arguments are an int, a float, and two strs, respectively).
ans `False`
17. True or False: All of the following are acceptable arguments for the float() function: 5,
5.0, "5", and "5.0".
ans `True`
18. True or False: All of the following are acceptable arguments for the eval() function: 5,
5.0, "5", and "5.0".
ans  `False`
19. True or False: The string "5.0, 6.0" is an acceptable argument for the eval() function
but not for the float() function.
ans `True`
