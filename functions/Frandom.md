# This is the line-by-line documentation for Frandom.py


## Imports
there are two imports:
```
import json
import random
```
these are used to import the default python json library and the default random library

The Python docs for random are here: https://docs.python.org/3/library/random.html
The Python docs for json are here: https://docs.python.org/3/library/json.html

## functions

All of the functions are identical except for some name and variable changes, here is the base template
```
class foo:
    def foo():
        with open("json-files/foo.json", "r") as file:
            data = json.load(file)
            foo = data['foo']['foo']
            return random.choice(foo)
```

At the beginning we are defining a class and function, with whatever relevant name.
Then with the line
``` 
with open("json-files/foo.json", "r") as file
```
We open the relevant JSON file, which is mostly random.json in read mode as the variable ```file```
With the line
```
data = json.load(file)
```
We are loading the contents of ```file``` into Python
Then, with the line
```
foo = data['foo']['foo']
```
It sets the relevant foo variable to the data needed for the specific function
and finally it returns a random choice from the dataset loaded in the last line with
```
return random.choice(foo)
```
