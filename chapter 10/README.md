## Review Questions (pase 252)
1. Assume the file input.txt is opened successfully in the following. What is the type of
    the variable z after the following code is executed:
    ```py
        file = open("input.txt", "r")
        z = file.readlines()
    ```
    - [x] (a) list
    - [ ] (b) str
    - [ ] (c) file object
    - [ ] (d) None of the above.
    - [ ] (e) This code produces an error.
    For problems 2 through 9, assume the file foo.txt contains the following:
    ```
    This is
    a test.
    Isn’t it? I think so.
    ```
2. What output is produced by the following?
    ```py
        file = open("foo.txt", "r")
        s = file.read()
        print(s[2])
    ```
    output: 
    ```py
    i
    ```
3. What output is produced by the following?
    ```py
        file = open("foo.txt", "r")
        file.readline()
        print(file.readline(), end="")
    ```
    output: 
    ```py
        a test 
    ```
4. What output is produced by the following?
    ```py
        file = open("foo.txt", "r")
        for line in file:
            print(line[0], end="")
    ```
    output:
    ```py
        TaI
    ```
5. What output is produced by the following?
    ``` py
        file = open("foo.txt", "r")
        s = file.read()
        xlist = s.split()
        print(xlist[1])
    ```
    output: 
    ```py
    is
    ```
6. What output is produced by the following?
    ```py
        file = open("foo.txt")
        s = file.read()
        xlist = s.split('\n')
        print(xlist[1])
    ```
    output: 
    ```py 
        a test.
    ```
7. What output is produced by the following?
    ```py
        file = open("foo.txt")
        xlist = file.readlines()
        ylist = file.readlines()
        print(len(xlist), len(ylist))
    ```
    output:
    ```
    3 0 
    ```
8. What output is produced by the following?
    ```py
        file = open("foo.txt")
        xlist = file.readlines()
        file.seek(0)
        ylist = file.readlines()
        print(len(ylist), len(ylist))
    ```
    output:
    ```
        3 3 
    ```
9. What output is produced by the following?
    ```py
        file = open("foo.txt")
        for x in file.readline():
        print(x, end=":")
    ```
    output: 
    ```py
       T:h:i:s: :i:s:; 
    ```
10. What is contained in the file out.txt after executing the following?
    ```py
        file = open("out.txt", "w")
        s = "this"
        print(s, "is a test", file=file)
        file.close()
    ```
    output: 
    ```
        this is a test 
    ```
11. What is contained in the file out.txt after executing the following?
    ```py
        file = open("out.txt", "w")
        s = "this"
        file.write(s, "is a test")
        file.close()
    ```
    ```
    The
    file will be empty since there is an error that prevents the write() method from being used—
    write() takes a single string argument and here is is given two arguments.;
    ```
12. What is contained in the file out.txt after executing the following?
    ```py
        file = open("out.txt", "w")
        s = "this"  
        file.write(s + "is a test") 
        file.close()
    ```
    output:
    ```
    this is a  test
    ```
13. What is contained in the file out.txt after executing the following?
    ```py
        file = open("out.txt", "w")
        s = "this"
        file.write("{} {}\n".format(s, "is a test"))
        file.close()
    ```
    output:
    ```
        this is a test
    ```