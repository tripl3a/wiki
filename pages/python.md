# Python

## String Formatting

See https://pyformat.info/

Thousand separator in format string with floats:
```
>>>'{0:,.2f}'.format(123466666)
'123,466,666.00'
```

## Check Version of Python Module

```bash
$ pip freeze | grep lxml
lxml==2.3
```

or

```python
>>> import statlib
>>> print(statlib.__version__) 
```