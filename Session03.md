<!-- $theme: default -->
<!-- footer: #pythonclub - 03  -->
<!-- $size: 16:9 -->

# pythonclub 03

<img src="images/importantigravity.PNG" alt="drawing" />

---

# pythonclub 03

Start your VM, open your terminal (`Ctrl+Alt+T`) and try to type the commands shown on screen, we're going to go through:

* functions


---

# functions

> A function is a group of connected statements (code) that perform a specific task.

```python
def function_name( input_variables ):
   something happens
   if something is True:
       then something else
   else:
       stuff here
   then, other thing happen
   maybe even another thing
   return output_variables
```

* Functions help break our code into **smaller** and **modular** parts. 
* Functions make larger codes more **organized** and **manageable**
* A function does not necessarily **return** something

---

# functions

Let's write a function which tells us if today is Monday.
We will use the `datetime` package (provided with python), open your python shell:

* `date` refers to the `datetime` package, which contains a function, `today()`, which returns today's date, try it:

```python
>>> from datetime import date
>>> date.today()
>>> datetime.date(2019, 1, 28)
```
* `datetime` also provides a function which finds the day of the week for a specific date (https://docs.python.org/3/library/datetime.html#datetime.date.weekday):
```python
>>> from datetime import date
>>> date.today().weekday()
>>> 0 #Because I executed this on a Monday (the 28th of January)
```
<!-- *footer: https://docs.python.org/3/library/datetime.html#datetime.date.weekday  -->

---

# functions

Now that we're able to determine if today is a Monday or not, let's write our function:

* Our function will take the date as an `input_variable`
* It will return a certain message if it is Monday and a different one if it isn't

```
from datetime import date

def monday_check(specimen_date):
    if specimen_date.weekday() == 0:
        message = "Monday again ... Go away Monday!"
    else:
        message = "Today is not a Monday!"
    return message
```
---

# functions
Let's now call our function in our script *(to execute a script `python3 script.py`)*:
```
#IMPORTS
from datetime import date

#FUNCTIONS
def monday_check(specimen_date):
    if specimen_date.weekday() == 0:
        message = "Monday again ... Go away Monday!"
    else:
        message = "Today is not a Monday!"
    return message

#SCRIPT
print("This program will tell you if it is already the worst day of the week.")
today = date.today()
print( monday_check(today) )
```
Try this code: https://github.com/pythonclubmtl/learning_python3 -> `ex_mondaycheck.py`
 
 <!-- *footer: false -->
 
 ---
 
 