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

*pass* is used to fill in a statement and do nothing at all. 

```
>>> class Empty_Class: pass
...
>>> object_ = Empty_Class()
>>> object_.value = 1
>>> object_.value
1
>>>
```

*del* is used to delete a variable or an object.

```
>>> del object_
>>> object_.value
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'object_' is not defined
>>>
```

*return* does exactly what it means literally. By default, a function in Python will return "None" if a return statement is not specified.

*yield* returns one item at a time and its companion function - *next* will emit each time when called, like a vending machine.

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

*break* is used to break out of a loop.

_**continue**_ is similar to *break* but instead of breaking out of the loop, it starts a new iteration of the loop.

