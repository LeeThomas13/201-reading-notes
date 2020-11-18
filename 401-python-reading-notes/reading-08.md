[List Comprehension](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)

List comprehensions provide a concise way to create lists. 

it consists of brackets containing an expresion followed by a for clause, then zero or more for or if clauses.

new_list = [expression(i) for i in old_list if filter(i)]

basic syntax: [ expression for item in list if conditional ]


create a simple list:
x = [i for i in range(10)]
print x

# This will give the output:
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)