# Ex 6e:Method Overriding in Two Separate Classes

## AIM:
To write a Python program that creates two different classes with the same method name info(), and invokes each method using their respective class objects.
## ALGORITHM:
1) Start the program.
2) Create a class Employee with:
  • Variables for name and department
  • Method info() to display employee details
3) Create another class Admin with:
  • Variables for name and department
  • Method info() to display admin details
4) Create an object of the Employee class.
5) Create an object of the Admin class.
6) Call the info() method using the Employee class object.
7) Call the info() method using the Admin class object.
8) End the program.

## PROGRAM:
```
class Employee:
    def __init__(self, name, dept):
        self.name = name
        self.dept = dept

    def info(self):
        print(f"{self.name} from {self.dept}")


class Admin:
    def __init__(self, name, dept):
        self.name = name
        self.dept = dept

    def info(self):
        print(f"{self.name} from {self.dept}")


e = Employee("Rooney", "Electronics")
a = Admin("Kalesh", "CS")

e.info()
a.info()

```

## OUTPUT
<img width="461" height="131" alt="image" src="https://github.com/user-attachments/assets/07156232-8fa3-42ef-afd4-262f804cadbc" />

## RESULT
Thus, the Python program successfully demonstrated two separate classes having the same method name, and the method info() was invoked using their respective objects.
