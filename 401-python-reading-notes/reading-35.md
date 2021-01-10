[Dunder Methods](https://dbader.org/blog/python-dunder-methods)

Dunder methods let you emulate the behavior of built-in types. For example, to get the length of a string you can call len('string'). But an empty class definition doesn’t support this behavior out of the box:

The constructor takes care of setting up the object. In this case it receives the owner name, an optional start amount and defines an internal transactions list to keep track of deposits and withdrawals.

use __str__, __repr__ to represent the object.

use __len__, __getitem__, __reversed__ to iterate through the object



[Iterators](https://dbader.org/blog/python-iterators)

how do for-in loops work in python?
well its simply syntactic sugar for a simple while loop.
ex:
repeater = Repeater('Hello')
iterator = repeater.__iter__()
while True:
    item = iterator.__next__()
    print(item)

we can simplify that to:
class Repeater:
    def __init__(self, value):
        self.value = value

    def __iter__(self):
        return self

    def __next__(self):
        return self.value


when using these loops python used a Stop Iteration exception once weve exhausted all unique character's in the list.

There is also a bounded interator that stop asfter a certain number of iterations.

Python Iterators – A Quick Summary
Iterators provide a sequence interface to Python objects that’s memory efficient and considered Pythonic. Behold the beauty of the for-in loop!
To support iteration an object needs to implement the iterator protocol by providing the __iter__ and __next__ dunder methods.
Class-based iterators are only one way to write iterable objects in Python. Also consider generators and generator expressions.

[Generators](https://dbader.org/blog/python-generators)

instead of writing all these iterator s by hand python has something called generators that do teh heavy lifting for you.

Generators look like normal functions, but their behavior is quite different. For starters, calling a generator function doesn’t even run the function. It merely creates and returns a generator object.

Yield and return statements seem like the same, but a return passes control back to the caller of thee function permanently. A yield returns control back onlny temporarily.

How to stop a generator function from going infinite:
Thankfully, as programmers we get to work with a nicer interface this time around. Generators stop generating values as soon as control flow returns from the generator function by any means other than a yield statement. This means you no longer have to worry about raising StopIteration at all!

Python Generators – A Quick Summary
Generator functions are syntactic sugar for writing objects that support the iterator protocol. Generators abstract away much of the boilerplate code needed when writing class-based iterators.
The yield statement allows you to temporarily suspend execution of a generator function and to pass back values from it.
Generators start raising StopIteration exceptions after control flow leaves the generator function by any means other than a yield statement.


[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)