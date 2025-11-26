# Ex 6c:Abstract Class:Abstract Class Invoice with Method Overriding
## AIM
To write a Python program that creates an abstract class Invoice with an abstract method invoice(), and two child classes that implement this method. Then invoke the methods using an object.
## ALGORITHM
1) Start the program.
2) Import ABC and abstractmethod from the abc module.
3) Create an abstract class Invoice containing an abstract method invoice().
4) Create a derived class SalaryInvoice that:
  • Implements the invoice() method for salary payment.
  • Prints the payment details and returns True.
5) Create another derived class ProductInvoice that:
  • Implements the invoice() method for product purchase.
  • Prints purchase details and returns True.
6) Create objects for both child classes.
7) Invoke the invoice() method using these objects.
8) Display the results.
9) End the program.
## Program
```
from abc import ABC, abstractmethod

class Invoice(ABC):

    @abstractmethod
    def invoice(self, amount):
        pass


class Salary(Invoice):
    def invoice(self, amount):
        print("paycheque of- ", amount)
        print("Purchase of the product- ", amount)
        print(True)


class Card(Invoice):
    def invoice(self, amount):
        print("pay through card of- ", amount)
        print("Purchase of the product- ", amount)
        print(True)


aa = Salary()
bb = Card()

aa.invoice(6500)
bb.invoice(2600)


```
## Output
<img width="543" height="212" alt="image" src="https://github.com/user-attachments/assets/3d75ec75-8f47-4aa0-b217-c57843a0d2aa" />

## Result
Thus, the program successfully demonstrated abstraction, inheritance, and method overriding using an abstract class Invoice and its child classes.
