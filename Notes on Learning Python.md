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

## Sequences
A sequence is a positionally ordered collection of other objects i.e. a group of objects that are arranged in an order.
Strings, lists and tuples are all sequences.
Common operations of sequences:
- len(x) returns the number of elements in the group
- indexing e.g. s[n_index] to retrieve the item in n position
- slicing e.g. s[i:j] to obtain items from i position up to but excluding j position
- concatenation e.g. '+'
- repetition e.g. '*'

These generic operations show up as built-in functions or expressions (e.g. len(x)) but type specific operations are called method calls (e.g. string.upper())

### Strings
```
>>> S = 'spam'
>>> S
'spam'
>>> len(S)
4
>>> S[0]
's'
>>> S[1]
'p'
>>> S[:]
'spam'
```


To change a string's value,

S = spam

1) Built-in / Sequence Operations 

```
L = list(S) 
L[1] = 'c' 
''.join(L) = scam
```


2) String Methods
```
S.replace('pa', 'XYZ')
S
>>> sXYZam
```

Note: The original string has not been changed (as strings are immutable) but rather new strings 'scam' and 'sXYZam' are being created.

### Numbers



