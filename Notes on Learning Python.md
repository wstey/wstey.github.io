# Notes on Learning Python by Mark Lutz

What makes up a Python program: 
1. Programs are composed of modules.
2. Modules contain statements.
3. Statements contain expressions.
4. Expressions create and process objects.

(Program > Modules > Statements > Expressions > Objects)

Everything we process in Python programs is a kind of object. A variable is a name that refers to a Python object. 
Every object has a: 
- data type (e.g. int)
- size (e.g. 4 bytes)
- value (e.g. 10)
- location in the computer's memory

A representation of the memory location of the object can be obtained by calling the function, id (e.g. id(variable_name).

A program cannot change an object's type or location, but some data types allow Python statements to change its value (e.g. list)

Polymorphism: In Python, the meaning (and operation) of the function depends on the underlying object type. For instance:

| Operations  | Numbers | Strings| Lists|
| ------------- | ------------- | ------------- | ------------- |
| '+' | addition: 1+2=3 | concatenation: '1' + '2' = '12' | concatenation: [1] + [2] = [1, 2]|
| '*' | multiplication: 1*2=2 | repetition: '1' * 2 = '11' | repetition: [1]*2 = [1, 1]|



## Python's Core Data Types
Python comes with built-in data structures that makes programming in Python easier and more efficient. Some of the basic types are introduced in the following table.


| Core Data Types  | Example literals/creation | Properties|
| ------------- | ------------- | ------------- |
| Numbers e.g. int/float/complex  | 1234, 3.1415, 3+4j, Decimal, Fraction  | Immutable |
| Strings  | single/double quotes (''),(""); str(object) | Immutable, Sequence|
| Lists  | [1, ['abc', 'def'],2]; list() | Sequence, Can be nested|
| Dictionaries  | {'food': 'spam', 'taste': 'yum'}, dict(key=value)|Mapping, Can be nested|
| Tuples  | (1,) | Immutable, Sequence, Can be nested|
| Sets  | {'i', 'j'}; set() | |
| Files  | myfile = open('eggs', 'r') | |

### Strings



