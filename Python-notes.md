# Python
## Intro to python
### Printing, data types and variables=== * To display a text, we use the *print* statement
```py
   print("display text")
```
* To store a value, one can use variable. Variables in python need no definition explicitly
```py
   variable_name = 56
   variable_name_2 = "string"
```
* Variable names cannot start with a number and in python we use underscores to seperate the words (snake_case)
* Variable names where the value is static is usally named in all uppercase like PI = 3.14159 (it's only a convention, nothing to relate it with a static variable)
* Integer is a whole number whereas floats are numbers with a decimal point
```py
   #Python comment is following by #
   whole_num = 54
   deci_num = 3.24342
```
* Mathematical operations follows the BODMAS rule
* Division in python always results float. In order to return an integer(does not round off, just removes the decimal place), we use *//*
```py
   float_division = 12/3 # returns 4.0 float value
   int_division = 12//3 # returns 4 integer value
```
### Strings
* To define a string, we can either use single or double quotation marks
```py
   print("Hey, it's me") # since we have single quotation marks in the inside we can use double quotes to mark the string
   print('he said, "blah.."') # similar to the above case
   print("he said, \"blah... \"") # one can use \ backslash as an escape character to signal a string
}}}
* Multiple lines can also we stored using *"""*
```py
   print("""
   
   First para
   second para
   """)
   """
   This can be used as a multi-line comment as python will process this as a string but since it doesnt get stored anywhere it can be used to write comments
   """
```

