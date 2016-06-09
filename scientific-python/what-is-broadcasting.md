## What is broadcasting in numpy?

This concept helps in resolving the matrix for situations where we have arrays
of different shapes. Smaller array broadcast/stretch over bigger array so as to
get comaptible shape arrays.

According to numpy docs, it helps in vectorising array operations so that 
looping occurs in C and not in python. It is usually efficient since we
stretch the scalar to the shape of the greater shape and hence less memory
is required. It happens so because it involves implicit copying of variable. 

Though, the process is quiet optimised in numpy but it usually leads to slow 
computations in case memory assignment is not taken care of.

**Rule:-** Two dimensions are compatible when they are equal or one of them is 
1.

The easiest example would be multiplying a scalar with a matrix.

And the case where you are most likely to get a ValueError exception is when the 
trailing dimensions are unequal.   

``` python 

a = np.array([1, 2])
b = np.array([5, 2, 7])

# Try a+b, it will throw ValueError.

c = a[:,np.newaxis]
c+b
# This will work according to the rules. 

``` 
