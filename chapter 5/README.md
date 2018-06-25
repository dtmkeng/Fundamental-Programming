## Class define 
```
class <ClassName>:
 <body>
```
### example
class statement that defines the `Patient` class where a Patient has a name,
`age`, and `malady` Each of these attributes is given a default value
```python
        1 >>> class Patient:
        2 ... name = "Jane Doe"
        3 ... age = 0
        4 ... malady = "healthy"
        5 ...
        6 >>> # Create an instance of a Patient with identifier of sally.
        7 >>> sally = Patient()
        8 >>> # Show sally’s name attribute.
        9 >>> sally.name
        10 ’Jane Doe’
        11 >>> # Set the name, age, and malady attributes for sally.
        12 >>> sally.name = "Sally Smith"
        13 >>> sally.age = 21
        14 >>> sally.malady = "bruised ego"
        15 >>> # Show sally’s name, age, and malady attributes.
        16 >>> print(sally.name, sally.age, sally.malady, sep="; ")
        17 Sally Smith; 21; bruised ego
        18 >>> def show(patient):
        19 ... print(patient.name, patient.age, patient.malady, sep="; ")
        20 ...
        21 >>> show(sally)
        22 Sally Smith; 21; bruised ego
```
### Creating a Class: Methods
```python
        1 >>> class Patient:
        2 ... name = "Jane Doe"
        3 ... age = 0
        4 ... malady = "healthy"
        5 ...
        6 ... def display(self):
        7 ... print("Name = ", self.name)
        8 ... print("Age = ", self.age)
        9 ... print("Malady = ", self.malady)
        10 ...
        11 >>> samuel = Patient()
        12 >>> samuel.name = "Samuel Sneed"
        13 >>> samuel.age = 18
        14 >>> samuel.malady = "broken heart"
        15 >>> samuel.display()
        16 Name = Samuel Sneed
        17 Age = 18
        18 Malady = broken heart
```
### The dir() Function
You can think of dir() as providing a directory of sorts.

```python
        19 >>> type(Patient)
        20 <class ’type’>
        21 >>> type(samuel)
        22 <class ’__main__.Patient’>
        23 >>> type(samuel.age)
        24 <class ’int’>
        25 >>> type(samuel.display)
        26 <class ’method’>
        27 >>> dir(samuel)
        28 [’__class__’, ’__delattr__’, ’__dict__’, ’__doc__’, ’__eq__’,
        29 ’__format__’, ’__ge__’, ’__getattribute__’, ’__gt__’, ’__hash__’,
        30 ’__init__’, ’__le__’, ’__lt__’, ’__module__’, ’__ne__’, ’__new__’,
        31 ’__reduce__’, ’__reduce_ex__’, ’__repr__’, ’__setattr__’,
        32 ’__sizeof__’, ’__str__’, ’__subclasshook__’, ’__weakref__’, ’age’,
        33 ’malady’, ’name’, ’display’]
```
###  The init () Method
Hence init () serves as the initialization method
```python
    this.value = self.value // java , python
```

```python
        >>> class Patient:
        2 ... def __init__(self, name, age, malady):
        3 ... """Initialize the Patient’s name, age, and malady."""
        4 ... self.name = name
        5 ... self.age = age
        6 ... self.malady = malady
        7 ...
        8 ... def display(self):
        9 ... """Display the Patient’s attributes."""
        10 ... print("Name = ", self.name)
        11 ... print("Age = ", self.age)
        12 ... print("Malady = ", self.malady)
        13 ...
        14 ... def cure(self):
        15 ... """Cure the Patient."""
        16 ... self.malady = "healthy"
        17 ...
        18 >>> sally = Patient("Sally Smith", 21, "bruised ego")
        19 >>> sally.display()
        20 Name = Sally Smith
        21 Age = 21
        22 Malady = bruised ego
        23 >>> sally.cure()
        24 >>> sally.display()
        25 Name = Sally Smith
        26 Age = 21
        27 Malady = healthy
```
Create new object
```python 
sally = Patient("Sally Smith", 21, "bruised ego")
```
In many respects we can think of it as being equivalent to a function call that looks like
```python
    __init__(sally, "Sally Smith", 21, "bruised ego")
```
### Operator Overloading
```python
        >>> s1 = "Hello" + " World!" # Concatenation.
        2 >>> print(s1)
        3 Hello World!
        4 >>> s2 = "&" * 70 # Repetition.
        5 >>> print(s1)
        6 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
        7 >>> 10 * "EI" + "-OH!" # Repetition and concatenation.
        8 ’EIEIEIEIEIEIEIEIEIEI-OH!’
        9 >>> s3 = "#" * 70.0
        10 Traceback (most recent call last):
        11 File "<stdin>", line 1, in <module>
        12 TypeError: can’t multiply sequence by non-int of type ’float’
```