## What is unicode, encode and decode?

Use encode whenever you want to convert unicode to string.
Use decode whenever you want to convert string to unicode.
Use unicode to typecast to unicode type. 

Also, it is print statement that does the magic. 

###How?

Try these 
```python 

string = 'Britannia Crème - Biscuit'
decoded_value = string.decode('utf-8')
print decoded_value
print type(decoded_value)
encoded_value = decoded_value.encode('utf-8')
print encoded_value
print type(encoded_value)

```

UnicodeDecodeError is an error which we usually get when processing such data 
with excel. It is so because Excel/xlswriter converts the data to ascii values
and when we use str to typecast, it breaks down. So, we can either typecast to
unicode or encode the value using utf-8 or any other desired encoding.
