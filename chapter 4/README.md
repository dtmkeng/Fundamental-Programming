## Review Questions (page 87)
1. The following code is executed
    ```python
        def f(x):
            return x + 2, x * 2
        x, y = f(5)
        print(x + y)
    ```
    What is the output produced by the print() statement?   
    - [ ] 7 10
    - [x] 17
    - [ ] x + y
    - [ ] This produces an error.
    - [ ] None of the above.
2. True or False: Names that are valid for variables are also valid for functions.
    ans  `True`
3. What output is produced by the print() statement when the following code is executed?
    ```python
        def calc_q1(x):
            q = 4 * x + 1
            return q
        calc_q1(5)
        print(q)
    ```
    - [ ] 24
    - [ ] 21
    - [ ] q
    - [x] This produces an error.
    - [ ] None of the above.
4. What is the value of q after the following code has been executed?
    ```python
        def calc_q2(x):
            q = 4 * x + 1
            print(q)
        q = calc_q2(5)
    ```
    - [ ] 24
    - [ ] 21
    - [ ] This produces an error.
    - [x] None of the above.
5. What is the value of q after the following code has been executed?
    ```python
        q = 20
        def calc_q3(x):
            q = 4 * x + 1
            return q
        q = calc_q3(5)
    ```
    - [ ] (a) 24
    - [x] (b) 21
    - [ ] (c) This produces an error.
    - [ ] (d) None of the above.
6. What is the output produced by the print() statement in the following code?
    ```python
        def calc_q4(x):
            q = 4 * x + 1
        print(calc_q4(5))
    ```
    - [ ] (a) 24
    - [ ] (b) 21
    - [ ] (c) q
    - [ ] (d) This produces an error.
    - [x] (e) None of the above.
7. What is the output of the print() statement in the following code?
    ```python
        abc = 5 + 6 // 12
        print(abc)
    ```
    - [ ] (a) This produces an error.
    - [ ] (b) 5 + 6 // 12
    - [x] (c) 5
    - [ ] (d) 5.5
    - [ ] (e) 6
8. What is the output of the print() statement in the following code?
    ```python
        def = 5 + 6 % 7
        print(def)
    ```
    - [x] (a) This produces an error.
    - [ ] (b) 5 + 6 % 7
    - [ ] (c) 11
    - [ ] (d) 4
9. The following code is executed:
    ```python
        def get_input():
            x = float(input("Enter a number: "))
            return x
        def main():
            get_input()
            print(x ** 2)
        main()
    ```
    At the prompt the user enters 2. What is the output of this program?
    - [ ] (a) x ** 2
    - [ ] (b) 4
    - [ ] (c) 4.0
    - [x] (d) This produces an error.
    - [ ] (e) None of the above.
10. The following code is executed:
    ```python
    def get_input():
        x = float(input("Enter a number: "))
        return x
    def main():
        print(get_input() ** 2)
    main()
    ```
    At the prompt the user enters 2. What is the output of this program?
    - [ ] (a) get_input() ** 2
    - [ ] (b) 4
    - [x] (c) 4.0
    - [ ] (d) This produces an error.
    - [ ] (e) None of the above.
11. What is the value of z after the following code is executed?
    ```python 
        def f1(x, y):
            print((x + 1) / (y - 1))
        z = f1(3, 3) + 1
    ```        
    - [ ] (a) 3
    - [ ] (b) 3.0
    - [ ] (c) 2
    - [x] (d) This produces an error.
12. What is the value of z after the following code is executed?
    ```python 
        def f2(x, y):
            return (x + 1) / (y - 1)
        z = f2(3, 3) + 1
    ```
    - [ ] (a) 3
    - [x] (b) 3.0
    - [ ] (c) 2
    - [ ] (d) This produces an error.
    - [ ] (e) None of the above.
13. What is the value of z after the following code is executed?
    ```python
        def f3(x, y = 2):
            return (x + 1) / (y - 1)
        z = f3(3, 3) + 1
    ```
    - [ ] (a) 3
    - [x] (b) 3.0
    - [ ] (c) 2
    - [ ] (d) This produces an error.
    - [ ] (e) None of the above.
14. What is the value of z after the following code is executed?
    ```python
        def f3(x, y = 2):
            return (x + 1) / (y - 1)
        z = f3(3) + 1
    ```
    - [ ] (a) 3
    - [ ] (b) 3.0
    - [ ] (c) 2
    - [ ] (d) This produces an error.
    - [x] (e) None of the above.
15. The following code is executed.
    ```python
        def inc_by_two(x):
            x = x + 2
            return x
        x = 10
        inc_by_two(x)
        print("x = ", x)
    ```
    What is the output produced by the print() statement?
    Ans `x = 10`
