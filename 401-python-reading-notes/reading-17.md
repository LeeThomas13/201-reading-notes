[Python Regular Expression Tutorial](https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial)

Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not. If you've ever used search engines, search and replace tools of word processors and text editors - you've already seen regular expressions in use. They are used at the server side to validate the format of email addresses or passwords during registration, used for parsing text data files to find, replace, or delete certain string, etc. They help in manipulating textual data, which is often a prerequisite for data science projects involving text mining.

when using regex with python you must import it as re

using the match() function will compare a desired pattern to an input. 

\+ Checks if the preceding character appears one or more times starting from that position.

\* Checks if the preceding character appears zero or more times starting from that position.

\? Checks if the preceding character appears exactly zero or one time starting from that position.

# Cheat Sheet

Character(s)	What it does
.	A period. Matches any single character except the newline character.
^	A caret. Matches a pattern at the start of the string.
\A	Uppercase A. Matches only at the start of the string.
$	Dollar sign. Matches the end of the string.
\Z	Uppercase Z. Matches only at the end of the string.
[ ]	Matches the set of characters you specify within it.
\	∙ If the character following the backslash is a recognized escape character, then the special meaning of the term is taken.
∙ Else the backslash () is treated like any other character and passed through.
∙ It can be used in front of all the metacharacters to remove their special meaning.
\w	Lowercase w. Matches any single letter, digit, or underscore.
\W	Uppercase W. Matches any character not part of \w (lowercase w).
\s	Lowercase s. Matches a single whitespace character like: space, newline, tab, return.
\S	Uppercase S. Matches any character not part of \s (lowercase s).
\d	Lowercase d. Matches decimal digit 0-9.
\D	Uppercase D. Matches any character that is not a decimal digit.
\t	Lowercase t. Matches tab.
\n	Lowercase n. Matches newline.
\r	Lowercase r. Matches return.
\b	Lowercase b. Matches only the beginning or end of the word.
+	Checks if the preceding character appears one or more times.
*	Checks if the preceding character appears zero or more times.
?	∙ Checks if the preceding character appears exactly zero or one time.
∙ Specifies a non-greedy version of +, *
{ }	Checks for an explicit number of times.
( )	Creates a group when performing matches.
< >	Creates a named group when performing matches.



[shutil](https://pymotw.com/3/shutil/)

shutil is for high level file operations.

By default when a new file is created under Unix, it receives permissions based on the umask of the current user. To copy the permissions from one file to another, use copymode().

shutil includes three functions for working with directory trees. To copy a directory from one place to another, use copytree(). It recurses through the source directory tree, copying files to the destination. The destination directory must not exist in advance.

The which() function scans a search path looking for a named file. The typical use case is to find an executable program on the shell’s search path defined in the environment variable PATH.

Python’s standard library includes many modules for managing archive files such as tarfile and zipfile. There are also several higher-level functions for creating and extracting archives in shutil. get_archive_formats() returns a sequence of names and descriptions for formats supported on the current system.

It can be useful to examine the local file system to see how much space is available before performing a long running operation that may exhaust that space. disk_usage() returns a tuple with the total space, the amount currently being used, and the amount remaining free.



[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)