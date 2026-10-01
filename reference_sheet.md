# Exam 1 Reference Materials

Topics:
1. [Print and formatting](#print-and-formatting)
2. [Variables and naming](#variables-and-naming)
3. [Data types](#data-types)
4. [Operators](#operators)
5. [Conditionals](#conditionals)
6. [Loops](#loops)
7. [Lists](#lists)
8. [Strings](#strings)

## Print and formatting
Use `"` or `'` for strings
- `print("Howdy, World!")` will output `Howdy, World!`
- `print('Howdy, World!')` will output `Howdy, World!`

Basic arithmetic
- `print(3 + 4)` will output `7`
- `print(1 / 2)` will output `0.5`
- `print(1 // 2)` will output `0`

Use a comma to print more than one item
- `print("howdy", 102, "20" + "25")` will output `howdy 102 2025`
- `print(1, 2, 3)` will output `1 2 3`
- `print(1, 2, 3, sep=":")` will output `1:2:3`
- `print(1, 2, 3, end=".")` will output `1 2 3.`

String concatenation is done with `+`
- `print("Howdy" + "World")` will output `HowdyWorld`

String repetition is done with `*`
- `print("Howdy" * 3)` will output `HowdyHowdyHowdy`

Escape characters use `\`
- `\t` for tab
- `\n` for a new line
- `\'` or `\"` for quotes

f-strings
- `print(f"The value of pi is {pi:.2f}")` will output `The value of pi is 3.14`, you must import pi from the math module first with `from math import *`
- `f"{2.3:<10}"` will create the string `2.3       `
- `f"{2.3:>10}"` will create the string `       2.3`
- `f"{2.3:^10}"` will create the string `    2.3     `

Math functions are imported from the math module
- `from math import *`
- `sqrt(x)` will calculate the square root of `x`
- `cos(x)`, `sin(x)`, `tan(x)` are trigonometric functions
- `acos(x)`, `asin(x)`, `atan(x)` are inverse trigonometric functions
- `log(x)` is the natural logarithm (base e, ln), `log10(x)` is base 10 logarithm
- Note: trig functions use radians (not degrees)

## Variables and naming
Python syntax for assigning variables
- the name of your variable is on the left, followed by the assignment operator (`=`), followed by the value to assign
- `<variable name> = <value>`

Variable naming
- Upper and lower case letters are valid
- Special characters are invalid, except `_`
- Numbers are valid except at the beginning of the name
- Python keywords are invalid
- `name2nd` is valid
- `2ndname` is invalid
- `myn@me` is invalid
- `_name` is valid

Values
- Values can be literals like `12`, `2.5`, `True`, or `"mystring"`
- Expressions will be evaluated and the result is assigned
- `mynum = 100 + 2` will store the value `102` in `mynum`
- `newnum = 25 / 5 - 3 * 4` will store the value `-7.0` in `newnum`
- `isbigger = 18 > 6` will store the value `True` in `isbigger`
- `bigstr = "big" * 5` will store the value `bigbigbigbigbig` in `bigstr`

Special assignment operators
- Will take the current value of the variable, modify it according to the operator, and reassign the new value
- `+=` will add the right hand side from the current value
- `-=` will subtract the right hand side from the current value
- `*=` will multiply the right hand side from the current value
- `/=` will divide the right hand side from the current value
- can also use `//=` for floor division and `%=` for modular division

## Data types
| Data Type | Examples |
| :---: | :--- |
| Integer | `4`, `-2`, `-5`, `10` |
| Floating-point (float) | `1.999`, `2.0`, `-4.89`, `867.5309` |
| Boolean | `True` evaluates to `1`, `False` evaluates to `0` |
| String | `"Letters"`, `'my string'` |

The `type` function will tell you the data type of a variable or expression
- `type(12)` evaluates to `int`
- `type(1.0)` evaluates to `float`
- `type(True)` evaluates to `bool`
- `type("False")` evaluates to `string`

`int(<value>)` converts a value to an integer
- `int("2")` evaluates to `2`
- `int(4.9)` evaluates to `4` because the number is truncated
- `int("3.0")` is an error

`float(<value>)` converts a value to a float
- `float(5)` evaluates to `5.0`
- `float("3.14")` evaluates to `3.14`
- `float("12")` evaluates to `12.0`

`str(<value>)` converts a value to a string
- `str(2.5)` evaluates to `"2.5"`
- `str(1)` evaluates to `"1"`
- `str(10 / 2)` evaluates to `"5.0"`

`bool(<value>)` converts a value to a Boolean
- `0`, `0.0`, `""` (empty string), and `[]` (empty list) convert to `False`
- All nonzero values convert to `True`
- `bool(-1)` evaluates to `True`
- `bool(0)` evaluates to `False`
- `bool(0.0)` evaluates to `False`
- `bool("")` evaluates to `False`

## Operators
Mathematical operators
- `+` addition
- `-` subtraction
- `*` multiplication
- `/` division
- `**` power / exponent
- `//` floor division, division without remainder
  - `7 // 3` evaluates to `2`
- `%` modulus, remainder from division
  - `7 % 3` evaluates to `1`

Order of operations (PEMDAS)
| Convention | Description |
| :---: | :--- |
| `()` | Items within parentheses are evaluated first |
| `**` | Exponentiation operators are evaluated next, the right side of the exponentiation is computed first |
| `*`, `/`, `//`, `%` | Next to be evaluated are `*`, `/`, `//`, and `%` |
| `+`, `-` | Finally come `+` and `-` with equal precendence |
| left-to-right | If more than one operator of equal precedence could be evaluated, evaluation occurs left to right |

Relational operators
- Compare two values
- `==` equality
- `!=` inequality
- `<` less than
- `>` greater than
- `<=` less than or equal to
- `>=` greater than or equal to

Boolean operators
- Operate on Boolean values (`True`, `False`)
- `not` flips the value
- `and` is `True` if and only if both values are `True`, otherwise `False`
- `or` is `False` if and only if both values are `False`, otherwise `True`
- `not` before `and` before `or`

*Mathematical operators > Relational operators > Boolean operators*

Other operators
- `is` identity operator, this is beyond the scope of ENGR 102
- `in` membership operator, determines if one string is a substring of another
  - `"a" in "aggies"` will evaluate to `True`
  - `"poo" not in "whoop"` will evaluate to `True`
- Note: these operators can also work on lists

## Conditionals
Python syntax for `if` statement
```python
if condition:
    # do this
```

If the condition evaluates to `True`, the indented code is executed

Use `if-else` when there are 2 possibilities
```python
if condition:
   # do this
else:
   # do this other thing
```

Use `if-elif-else` when there are more than 2 alternative paths
```python
if condition1:
    # do this first thing
elif condition2:
    # do this second thing
else:
    # do this third thing if all above conditions are False
```

Note: You can nest conditional statements

## Loops
There are 4 components to a loop:
1. Initialize a control variable
2. Determine the continuation condition
3. Things to do
4. Update the control variable

A `while` loop (conditional loop) repeats the indented code until the condition is `False`
```python
while condition:
    # do this
```

Example
```python
i = 0                        # 1. initialize the control variable i
while i < 10:                # 2. continuation condition
    print("Doing something") # 3. things to do
    i += 1                   # 4. update the control variable i
```
The variables `i`, `j`, and `k` are commonly used as control variables

A `for` loop (ranged loop) repeats the indented code for the specified instances
```python
for i in range(10):          # 1. initialize the control variable i, 2. continue for 10 iterations, 4. update the control variable i
    print("Doing something") # 3. things to do
```

A `for` loop is used when you have a known number of iterations, or when you want to iterate through a specific, known set of items. A `while` loop is used when you want to repeat an unknown number of iterations. For example, until a specific value is encountered or a general condition is met.

Range
- `range(n)` generates the sequence `0, 1, ..., n-2, n-1`
  - Note that the sequence starts at `0` and contains `n` elements
  - `range(10)` produces the sequence `0, 1, 2, 3, 4, 5, 6, 7, 8, 9`
- `range(start, stop)` starts at the value `start` and stops *before* the value `stop`
  - `range(1, 5)` produces the sequence `1, 2, 3, 4`
- `range(start, stop, step)` starts at the value `start`, stops *before* the value `stop`, and increments with a step size of `step`
  - `range(3, 10, 3)` produces the sequence `3, 6, 9`

## Lists
Python syntax for lists
```python
list_name = [element_0, element_1, ...]
```

You can append a value (add to the end) using the append list method
```python
list_name.append("add this")
```

You can also append a value using concatenation. Note: You can only concatenate lists with other lists
```python
grades = [87, 93, 75, 100, 82, 91, 85]
grades += [80] # concatenate a value to the list, put the value in [] to create a list containing that value
grades += ["a string", "98"] # can also concatenate multiple values at once
# grades += 100 # this will cause an error (cannot concatenate list with int)
print(grades)
```
will output `[87, 93, 75, 100, 82, 91, 85, 80, "a string", "98"]`

Python syntax for slicing lists
```python
list_name[a:b]
```

The resulting sublist will contain values from index `a` to index `b-1`
```python
# index    0   1   2   3   4   5   6
grades = [87, 93, 75, 100, 82, 91, 85]
print(grades[1:4])
```
will output `[93, 75, 100]`

You can change the step size with `list_name[start:stop:step]`
```python
# index    0   1   2   3   4   5   6
grades = [87, 93, 75, 100, 82, 91, 85]
print(grades[1:5:2])
```
will output `[93, 100]`

You can omit the start or stop values and it will slice from the beginning or go to the end
```python
# index    0   1   2   3   4   5   6
grades = [87, 93, 75, 100, 82, 91, 85]
print(grades[:3]) # this will slice the first 3 values in grades
print(grades[4:]) # this will slice the last 3 values in grades
print(grades[::-1]) # this will start at the beginning, go to the end, and print the list backward (negative step size)
```
will output
```
[87, 93, 75]
[82, 91, 85]
[85, 91, 82, 100, 75, 93, 87]
```

List methods (may show up on an exam)
- `len(x)` will return the number of elements in list `x`, also works on strings
- `min(x)` will return the minimum value in list `x`
- `max(x)` will return the maximum value in list `x`
- `sum(x)` will return the sum of all values in list `x`
- `mylist[start:end]` allows you to slice certain values in the list `mylist`
- `mylist.append(value)` will add `value` to the end of `mylist`
- `mylist.sort()` will sort the list from smallest to largest

List methods (reference only, NOT on an exam)
- `mylist.index(value)` will find the index of the first element in the list `mylist` with the matching `value`
- `mylist.count(value)` will find the number of occurrences of `value` in the list `mylist`
- `mylist.insert(index, value)` will insert `value` at index location `index`
- `del mylist[index]` will remove the item at index location `index` in `mylist`
- `mylist.pop()` will remove the last item in `mylist`
- `mylist.remove(value)` will remove the first instance of `value` in `mylist`

Example
```python
x = [0, 1, 2, 3]
print(len(x), min(x), max(x), sum(x))
```
will output `4 0 3 6`

Another example
```python
mylist = ["a", "b", "c", "d", "e", "a"]
print(mylist.index("b"), mylist.count("a"), mylist[1:4])
```
will output `1 2 ['b', 'c', 'd']`

Yet another example
```python
mylist = ["a", "b", "c", "d", "e"]
del mylist[1]         # removes element "b"
mylist.pop()          # removes element "e"
mylist.append("f")    # adds element "f" to end
mylist.insert(2, "z") # adds element "z" at index 2
print(mylist)
```
will output `['a', 'c', 'z', 'd', 'f']`

## Strings
You can slice strings similar to how you slice lists
```python
name = "Texas A&M   University      1876"
print(name[6:9], name[-4:])
```
will output `A&M 1876`

```python
mystr = "abcdefghijklmnopqrstuvwxyz"
print(mystr[3:9:2]) 
```
will output `dfh`

You can split a string into a list of strings using `<str>.split()`. By default, this will split on whitespace (space, tab, and newline characters).
```python
name = "Texas A&M   University      1876"
name_list = name.split() # split on the whitespace (spaces) to create a list
print(name_list)
```
will output `['Texas', 'A&M', 'University', '1876']`

You can join a list of strings into a single string using `<str>.join(<list of strings>)`
```python
name = "Texas A&M   University      1876"
name_list = name.split() # split on the whitespace (spaces) to create a list
new_name = " ".join(name_list) # using exactly one space " "
print(new_name)
```
will output `Texas A&M University 1876`

You can remove leading and trailing whitespace from a string using `<str>.strip()`
```python
mystr = "      blue sky   ".strip() # this will remove the spaces at the beginning and end (NOT the middle)
print(mystr)
```
will output `blue sky`

Revised Fall 2026 SNR
