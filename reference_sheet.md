# Exam 1 Reference Materials

Topics:
1. [Print and formatting](#print-and-formatting)
2. [Variables and naming](#variables-and-naming)
3. [Data types](#data-types)
4. [Operators](#operators)
5. [Conditionals](#conditionals)
6. [Loops](#loops)
7. [Lists](#lists)

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

## Loops

## Lists

Revised Fall 2026 SNR
