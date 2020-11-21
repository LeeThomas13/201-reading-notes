[Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

Accessing Object Variables:

To access the variable inside of the newly created object "myobjectx" you would do the following:

class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

myobjectx.variable

Accessing Object Functions:

To access a function inside of an object you use notation similar to accessing a variable:



class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

myobjectx.function()

Example Problem:

We have a class defined for vehicles. Create two new vehicles called car1 and car2. Set car1 to be a red convertible worth $60,000.00 with a name of Fer, and car2 to be a blue van named Jump worth $10,000.00.

# define the Vehicle class
class Vehicle:
    name = ""
    kind = "car"
    color = ""
    value = 100.00
    def description(self):
        desc_str = "%s is a %s %s worth $%.2f." % (self.name, self.color, self.kind, self.value)
        return desc_str
# your code goes here

# test code
print(car1.description())
print(car2.description())

[Thinking Recursively](https://realpython.com/python-thinking-recursively/)

Problems (in life and also in computer science) can often seem big and scary. But if we keep chipping away at them, more often than not we can break them down into smaller chunks trivial enough to solve. This is the essence of thinking recursively,

Maintaining State
When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:

Thread the state through each recursive call so that the current state is part of the current call’s execution context
Keep the state in global scope

Recursive Data Structures in Python
A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure.


[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)