## What is split and partition in python?

Split returns a list of words separated by a delimiter. There is an optional
maxsplit which if specified gives the maximum number of occurences of 
delimiter until which it should split.

Partition returns a 3-tuple containing the part before the separator, the 
separator itself, and the part after the separator. It throws TypeError when 
nothing is passed and ValueError when empty string is passed as parameter.

``` python 

# Split 
a = 'a:b:c'
a.split()
a.split(':')
a = 'a:b:c b'
a.split()
a.split(':', 1)
a.split(':', 2)
a.split(':', 3)

# Partition
# Throws TypeError 
# a.partition()
# Throws ValueError
# a.partition('')
a.partition(' ') 
a = 'abc'
a.partition(' ')

```

