## How to perform string operation on every row in pandas?

Be it a dataframe or a series object, when it comes to performing
python string operations on every row in pandas we have to use the 
.str attribute on the object. 

For my use case, each row was a review (string) and I had to convert 
each row to a list of words in the review. All I wanted was to perform
review.split(" "). But since the review was a Series object and split was
a string method, I had to convert each row to str first as given below
review.str.split(" ").

```python 
import pandas as pd
series_obj = pd.Series(["sancheeta", "kaushal", "saksham", "kaushal"])
series_obj.columns 

# Convert all the entries to title case
print series_obj.str.title()

``` 