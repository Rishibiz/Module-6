# Ex 6a:Polymorphism:Method Overriding in Inheritance (Vehicle → Car)

## AIM
To write a Python program that demonstrates method overriding by creating a parent class Vehicle and a child class Car that overrides the methods max_speed() and change_gear().

## ALGORITHM
1) Start the program.
2) Create a parent class Vehicle with:
  • show() → to display model, color, and price
  • max_speed() → prints base max speed
  • change_gear() → prints base gear info
3) Create a child class Car inheriting from Vehicle.
4) Override max_speed() in Car to print the car-specific max speed.
5) Override change_gear() in Car to print the car-specific gear change.
6) Create objects for Car and Vehicle.
7) Call their methods to show the effect of method overriding.
8) End the program.

## Program
```
class Vehicle:
    def __init__(self, name, model, color, price):
        self.name = name
        self.model = model
        self.color = color
        self.price = price

    def show(self):
        print(f"Details: {self.name} {self.model} {self.color} {self.price}")

    def max_speed(self):
        print("Vehicle max speed is 150")

    def change_gear(self):
        print("Vehicle change 6 gear")


class Car(Vehicle):
    def max_speed(self):
        print("Car max speed is 240")

    def change_gear(self):
        print("Car change 7 gear")


c = Car("Car", "x1", "Red", 20000)
c.show()
c.max_speed()
c.change_gear()

t = Vehicle("Truck", "x1", "white", 75000)
t.show()
t.max_speed()
t.change_gear()

```
## Output
<img width="564" height="212" alt="image" src="https://github.com/user-attachments/assets/21775242-6638-4924-9da0-09cb17001a8f" />

## Result
Thus, the program successfully demonstrates method overriding where the Car class overrides the methods of the Vehicle class.
