## How to perform string operation on every row in pandas?

Be it a dataframe or a series object, when it comes to performing
python string operations on every row in pandas we have to use the 
.str attribute on the object. 

```python 
import pandas as pd
series_obj = pd.Series(["sancheeta", "kaushal", "saksham", "kaushal"])
series_obj.columns 

# Convert all the entries to title case
print series_obj.str.title()

``` 