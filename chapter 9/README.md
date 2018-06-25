## Review Questions (page 231)
1. What is printed by the following Python fragment?
    ```py
        s = "Jane Doe"
        print(s[1])
    ```
    - [ ] (a) J
    - [x] (b) e
    - [ ] (c) Jane
    - [ ] (d) a
2. What is printed by the following Python fragment?
    ```py
        s = "Jane Doe"
        print(s[-1])
    ```
    - [ ] (a) J
    - [x] (b) e
    - [ ] (c) Jane
    - [ ] (d) a
3. What is printed by the following Python fragment?
    ```py
        s = "Jane Doe"
        print(s[1:3])
    ```
    - [ ] (a) Ja
    - [ ] (b) Jan
    - [ ] (c) an
    - [ ] (d) ane
4. What is the output from the following program, if the input is Spam And Eggs?
    ```py
        def main():
            msg = input("Enter a phrase: ")
            for w in msg.split():
                print(w[0], end="")
        main()
    ```
    - [x] (a) SAE
    - [ ] (b) S A E
    - [ ] (c) S S S
    - [ ] (d) Spam And Eggs
    - [ ] (e) None of the above.
5. What is the output of this program fragment?
    ```py
        for x in "Mississippi".split("i"):
            print(x, end="")
    ```
    - [x] (a) Msssspp
    - [ ] (b) M ssissippi
    - [ ] (c) Mi ssi ssi ppi
    - [ ] (d) M ss ss pp
6. ASCII is
    - [x] (a) a standardized encoding of written characters as numeric codes.
    - [ ] (b) an encryption system for keeping information private.
    - [ ] (c) a way of representing numbers using binary.
    - [ ] (d) computer language used in natural language processing.
7. What function can be used to get the ASCII value of a given character?
    - [ ] (a) str()
    - [x] (b) ord()
    - [ ] (c) chr()
    - [ ] (d) ascii()
    - [ ] (e) None of the above.
8. What is output produced by the following?
    ```py
        s = "absense makes the brain shrink"
        x = s.find("s")
        y = s.find("s", x + 1)
        print(s[x : y])
    ```
    - [ ] (a) sens
    - [ ] (b) ens
    - [ ] (c) en
    - [x] (d) sen
9. One difference between strings and lists in Python is that
    - [ ] (a) strings are sequences, but lists aren’t.
    - [ ] (b) lists can be indexed and sliced, but strings can’t.
    - [x] (c) lists are mutable (changeable), but strings immutable (unchangeable).
    - [ ] (d) strings can be concatenated, but lists can’t.
10. What is an appropriate for-loop for writing the characters of the string s, one character per line?
    - [ ] (a) 
    ```py
        for ch in s:
            print(ch)
    ```
    - [ ] (b) 
    ```py 
        for i in range(len(s)):
            print(s[i])
    ```
    - [ ] (c) Neither of the above.
    - [x] (d) Both of the above.

11. The following program fragment is meant to be used to find the sum of the ASCII values for
    all the characters in a string that the user enters. What is the missing line in this code?
    ```py
        phrase = input("Enter a phrase: ")
        ascii_sum = 0 # accumulator for the sum
        for ch in phrase:
            ##### missing line here
        print(ascii_sum)
    ```
    - [ ] (a) ascii_sum = ascii_sum + ch
    - [ ] (b) ascii_sum = chr(ch)
    - [ ] (c) ascii_sum = ascii_sum + chr(ch)
    - [x] (d) ascii_sum = ascii_sum + ord(ch)
12. What is the result of evaluating the expression `chr(ord('A') + 2)`?
    - [ ] (a) 'A2'
    - [x] (b) 'C'
    - [ ] (c) 67
    - [ ] (d) An error.
    - [ ] (e) None of the above.
13. What is the output of the following code?
```py
    s0 = "A Toyota"
    s1 = ""
    for ch in s0:
        s1 = ch + s1
    print(s1)
```
- [ ] (a) A Toyota
- [x] (b) atoyoT A
- [ ] (c) None of the above.

14. What is the output of the following code?
    ```py
        s0 = "A Toyota" 
        s1 = ""
        for ch in s0[ : : -1]:
            s1 = ch + s1
        print(s1)
    ```
    - [x] (a) A Toyota
    - [ ] (b) atoyoT A
    - [ ] (c) None of the above.
15. What is the output of the following code?
    ```py
        s0 = "A Toyota"
        s1 = ""
        for ch in s0[-1 : 0 : -1]:
            s1 = s1 + ch
        print(s1)
    ```
    - [ ] (a) A Toyota
    - [ ] (b) atoyoT A
    - [x] (c) None of the above.
16. What is the value of z after the following has been executed:
    ```py
        s = ''
        for i in range(-1, 2):
            s = s + str(i)
        z = int(s)
    ```
    - [ ] (a) 0
    - [ ] (b) 2
    - [ ] (c) -1012
    - [x] (d) -101
    - [ ] (e) This code produces an error.

17. What is the value of ch after the following has been executed?
    ```py
        ch = 'A'
        ch_ascii = ord(ch)
        ch = chr(ch_ascii + 2)
    ```
    - [ ] (a) 'A'
    - [ ] (b) 67
    - [x] (c) 'C'
    - [ ] (d) This code produces an error.
18. What is the output produced by the print() statement in the following code?
    ```py
        s1 = "I’d rather a bottle in front of me than a frontal lobotomy."
        s2 = s1.split()
        print(s2[2])
    ```
    - [ ] (a) ’
    - [ ] (b) d
    - [ ] (c) rather
    - [x] (d) a
    - [ ] (e) bottle

19. What is the output produced by the print() statement in the following code?
    ```py
        s1 = "I’d\nrather a bottle in front of me than a frontal lobotomy."
        s2 = s1.split()
        print(s2[2])
    ```
    - [ ] (a) ’
    - [ ] (b) d
    - [ ] (c) rather
    - [x] (d) a
    - [ ] (e) bottle
    - [ ] (f) None of the above.
20. The variable s contains the string ’cougars’. A programmer wants to change this variable
    so that it is assigned the string ’Cougars’. Which of the following will accomplish this?
    - [ ] (a)
    `s.upper()`
    - [ ] (b)
    `s[0] = 'C'`
    - [x] (c)
    `s = 'C' + s[1 : len(s)]`
    - [ ] (d)
    `s.capitalize()`
    - [ ] (e) All of the above.
    - [ ] (f) None of the above.
21. What output is produced by the following code?
    ```py
        s = "Jane Doe"
        print(s[1 : 3: -1])
    ```
    - [ ] (a) aJ
    - [ ] (b) naJ
    - [ ] (c) na
    - [ ] (d) en
    - [x] (e) None of the above.

22. After the following commands have been executed, what is the value of x?
```py
    s = "this is a test"
    x = s.split()
```
output: 
```py
   ['this','is','test']
```
23. After the following commands have been executed, what is the value of y?
```py
    s = "this is a test"
    y = s.split("s")
```
output:
```py
    ['thi',' i a te','t']
```
24. Recall that the `str()` function returns the string equivalent of its argument. What is the
    output produced by the following:
    ```py
        a = 123456
        s = str(a)
        print(s[5] + s[4] + s[3] + s[2])
    ```
    output
    ```py
        6523
    ```
25. What is the value of `count` after the following code has been executed?
    ```py
        s = "He said he saw Henry."
        count = s.count("he")
    ```
    - [ ] (a) 0
    - [ ] (b) 1
    - [ ] (c) 2
    - [ ] (d) 3
    - [ ] (e) None of the above.
26. What is the value of s2 after the following has been executed?
    ```py
        s1 = "Grok!"
        s2 = s1[ : -2] + "w."
    ```
    - [x] (a) Grow.
    - [ ] (b) kw.
    - [ ] (c) k!w
    - [ ] (d) None of the above.
27. What is the value of s2 after the following has been executed?
    ```py
        s1 = "Grok!"
        s2 = s1[-2] + "w."  
    ```
    - [ ] (a) Grow.
    - [x] (b) kw.
    - [ ] (c) k!w
    - [ ] (d) None of the above.
28. What is the value of s2 after the following has been executed?
    ```py
        s1 = "Grok!"
        s2 = s1[-2 : ] + "w."
    ```
    - [ ] (a) kw.
    - [ ] (b) Grow.
    - [ ] (c) k!w
    - [x] (d) None of the above.