[Read & Write Files in Python](https://realpython.com/read-write-files-python/)

What is a file:
At its core, a file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.


One problem often encountered when working with file data is the representation of a new line or line ending. The line ending has its roots from back in the Morse Code era, when a specific pro-sign was used to communicate the end of a transmission or the end of a line.

open a file with open()

'r'	Open for reading (default)
'w'	Open for writing, truncating (overwriting) the file first
'rb' or 'wb'	Open in binary mode (read/write using byte data)

.readlines() method will print out 5 bytes of a line from the file.


Working With Two Files at the Same Time
There are times when you may want to read a file and write to another file at the same time. If you use the example that was shown when you were learning how to write to a file, it can actually be combined into the following:

d_path = 'dog_breeds.txt'
d_r_path = 'dog_breeds_reversed.txt'
with open(d_path, 'r') as reader, open(d_r_path, 'w') as writer:
    dog_breeds = reader.readlines()
    writer.writelines(reversed(dog_breeds))

[Exceptions in Python](https://realpython.com/python-exceptions/)

you can raise errors with the raise statement.

x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))

assert will test if a condition is true. great for testing.

the try and except blocks will run code and if a condition in that code is met the exception block will fire.

try:
    linux_interaction()
except:
    print('Linux function was not executed')


[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)