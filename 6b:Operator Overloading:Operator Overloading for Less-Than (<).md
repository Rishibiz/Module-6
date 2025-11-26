# Ex 6b:Operator Overloading:Operator Overloading for Less-Than (<)

## AIM
To write a Python program that overloads the less-than (<) operator using a class so that objects can be compared based on their values.
## ALGORITHM
1) Start the program.
2) Create a class A with an __init__() method to store a value.
3) Define the special method __lt__() to overload the less-than operator.
4) Inside __lt__(), compare the values of two objects and return True or False.
5) Create two objects: ob1 = A(2) and ob2 = A(3).
6) Use the < operator to compare the two objects.
7) Print the appropriate message based on the comparison.
8) End the program.
## Program
```
class A:
    def __init__(self, value):
        self.value = value

    def __lt__(self, other):
        return self.value < other.value


ob1 = A(2)
ob2 = A(3)

if ob1 < ob2:
    print("ob1 is less than ob2")
else:
    print("ob1 is not less than ob2")

```
## Output
<img width="428" height="129" alt="image" src="https://github.com/user-attachments/assets/eda17b66-e294-4260-9c2a-86604a0d28eb" />

## Result
Thus, the Python program successfully overloaded the less-than operator (<) to compare two objects based on their stored values.
