_**assert**_ is used to check if the expression is correct or not. It returns **AssertionError** if the expression is false.

```
>>> num = 4
>>> assert num == 4
>>> assert num == 5
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
AssertionError
>>>
```

_**pass**_ is used to fill in a statement and do nothing at all. 

```
>>> class Empty_Class: pass
...
>>> object_ = Empty_Class()
>>> object_.value = 1
>>> object_.value
1
>>>
```

_**del**_ is used to delete a variable or an object.

```
>>> del object_
>>> object_.value
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'object_' is not defined
>>>
```

_**return**_ does exactly what it means literally. By default, a function in Python will return **"None"** if a return statement is not specified.

_**yield**_ returns one item at a time and its companion function - _**next**_ will emit each time when called, like a vending machine.

```
>>> def long_list():
...     long_list = ["item1", "item2", "item3", "item4", "item5"]
...     for item in long_list:
...         yield item
...
>>> my_long_list = long_list()
>>> print(next(my_long_list))
item1
>>> print(next(my_long_list))
item2
>>> print(next(my_long_list))
item3
>>> print(next(my_long_list))
item4
>>> print(next(my_long_list))
item5
>>> print(next(my_long_list))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
StopIteration
>>>
```

_**break**_ is used to break out of a loop.

_**continue**_ is similar to _**break**_ but instead of breaking out of the loop, it starts a new iteration of the loop.

_**set**_ is a data type that holds only unique items. It will automatically remove duplicates.

```
>>> egg_set = set(["egg", "bacon", "egg"])
>>> type(egg_set)
<class 'set'>
>>> egg_set
{'egg', 'bacon'}
>>>
```

A _**tuple**_ is immutable. Once it is created, it cannot be changed.

```
>>> breakfast = ("egg", "soup")
>>> breakfast
('egg', 'soup')
>>> breakfast[1]
'soup'
>>> breakfast[0] = "bread"
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'tuple' object does not support item assignment
>>>
```

Use custom separation with _**print**_ function.

```
>>> print("This is a tab", "separation example", sep="\t")
This is a tab   separation example
>>>
```

power and exponent 

```
>>> import math
>>> math.pow(2,3)
8.0
>>> 2**3
8
>>> math.pow(2,4)
16.0
>>> 2**4
16
>>>
```

How to get type of a variable.

```
>>> number = 100
>>> type(number)
<class 'int'>
>>> type(number).__name__
'int'
>>> print(f"{number} is type {type(number).__name__}")
100 is type int
>>>
```

Round a decimal number.

```
>>> r = 1.234134243444
>>> round(r, 3)
1.234
>>>
```

