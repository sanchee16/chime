## What is append, extend and insert in list?

Append needs an object which will be added to the end of the list. 

Extend needs an iterable which adds all the elements to the end of the list.

Insert inserts an item at a specified position.

```python 

numbers = [1, 2, 3]
append_num = [5, 6]
numbers.append(append_num)
extend_num = [5, 6]
numbers.extend(extend_num)
numbers.insert(1, 2)
numbers.insert(1, [1, 2])

# Magic happens now.

words = []
words.extend('Computer Science')
words.append('Computer Science')

```
