## What does np.newaxis do? 

np.newaxis is used to create a new dimension in your array.

Question is when will we need it? We need it almost every time when we are 
using csv to load data and the data contains multiple features.So, in order to
process it with scikitlearn where we need a tuple for X. X being the indepen
-dent variable.

For example -

We load data into a variable dataset which has three features.
so we have dataset as array of arrays whose shape is (n_samples, n_features)
But what we need is dataset_X whose shape is (n_samples, 1) and n_samples 
must be the samples of a chosen feature.

So, all I need to do is dataset_X = dataset[:, np.newaxis, c]   
where c is the column number of the feature. Say, for feature_2 , c=1
and yes we are good to go and fit the data.
