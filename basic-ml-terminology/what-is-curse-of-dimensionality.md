## What is curse of dimensionality?

It is a phenomenon that arises when dealing with highly dimensional data. 

The root cause for the phenomenon is that as dimensions grow data
becomes **sparse** which in turn leads to bad statistical results
because statistics relies on patterns of data and it is really 
difficult to define patterns in sparse data.

According to Wikipedia, curse of dimensionality also depends on algorithm.

Additionally, the concept is closely related to _overfitting_. Here,
we try to balance the absence of patterns in sparse data by increasing the 
number of features under consideration which in turn deteriorates the
performance of classifier.
