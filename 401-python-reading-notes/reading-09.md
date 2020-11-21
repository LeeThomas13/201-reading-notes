[Dunder Methods](https://dbader.org/blog/python-dunder-methods)

dunder = 'double under'

Object initialization = To construct account objects from the Account class I need a constructor which in Python is the __init__ dunder:

Object representation = It’s common practice in Python to provide a string representation of your object for the consumer of your class (a bit like API documentation.) There are two ways to do this using dunder methods:

__repr__: The “official” string representation of an object. This is how you would make an object of the class. The goal of __repr__ is to be unambiguous.

__str__: The “informal” or nicely printable string representation of an object. This is for the enduser.

Object Iteration = __len__, __getitem__, __reversed__, __contains__

Operator Overloading for Comparing Accounts = __eq__
__lt__

Operator Overloading for Merging Accounts = __add__

Callable Python Objects = __call__

Context Manager Support and The With Statement = __enter__, __exit__

[Statistics-Probability](https://www.dataquest.io/blog/basic-statistics-in-python-probability/)

What is probability = its the percentabe that a certain outcome will happen.

Three sigma rule: The Three Sigma rule, also known as the empirical rule or 68-95-99.7 rule, is an expression of how many of our observations fall within a certain distance of the mean. 

Central Limit Theorem: If we make many estimates, the Central Limit Theorem dictates that the distribution of these estimates will look like a normal distribution.

Zscore: The Z-score is a simple calculation that answers the question, “Given a data point, how many standard deviations is it away from the mean?” The equation below is the Z-score equation. 

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)