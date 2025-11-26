# Ex 6d:Encapsulation:Display age using a class
## AIM
To write a Python program that creates a class with name and age variables and a method to display the age, then invoke it using an object.
## ALGORITHM

1) Start the program.
2) Create a class pub_mod with variables name and age.
3) Define a method display() to print the name and age.
4) Create an object of the class.
5) Assign values to name and age through the constructor.
6) Invoke the display method using the object.
7) End the program.

## Program
```
class pub_mod:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        print("Name: ", self.name)
        print("Age: ", self.age)


p = pub_mod("Jason", 35)

p.display()

```

## Output
<img width="353" height="131" alt="image" src="https://github.com/user-attachments/assets/96ff78c6-7825-4f4e-be04-48a0dff7b5c6" />

## Result
Thus, the Python program successfully created a class with name and age variables and displayed the age using a class method invoked through an object.
