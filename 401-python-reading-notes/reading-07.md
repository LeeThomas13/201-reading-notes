[Python Scope](https://realpython.com/python-scope-legb-rule/)
#Focus on Global and Nonlocal keywords

#Global
from the moment you fire a python  file you are in thee global scope, and the interpreter turns your main program into a module called __main__.


Note: In Python, the notions of global scope and global names are tightly associated with module files. For example, if you define a name at the top level of any Python module, then that name is considered global to the module. That’s the reason why this kind of scope is also called module scope.

You can access or referance any global name from any place in your code. This includes functions and classes.

Whenever you assign a value to a name in Python, you either crate a new name or update an existing name.


#nonlocal
nonlocal statements can be accessed within functions but not assigned or updated. Unlinke globalnyou cant use non local outside of a nested or enclosed function.to be more precise you cant use a nonlocal statement in either the global scope or in a local scope.


[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)