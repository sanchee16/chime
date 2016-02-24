## What does any/all mean in python?

any or all are python builtin function that check for truth values in
iterables or sequences. 

Their power lies in their basic nature of short circuiting.

Any stops after the first True value it sees and all stops after the 
first False value.

Any returns True if any element of the iterable is set to True. If the
iterable is empty, it returns False.

All returns True if all the elements are True.If the iterable is empty,
it returns True.

These functions also accept generator expressions.



