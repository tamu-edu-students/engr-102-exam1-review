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
- `f"{2.3:^10}"` will create the string `   2.3    `

Math functions are imported from the math module
- `from math import *`
- `sqrt(x)` will calculate the square root of `x`
- `cos(x)`, `sin(x)`, `tan(x)` are trigonometric functions
- `acos(x)`, `asin(x)`, `atan(x)` are inverse trigonometric functions
- `log(x)` is the natural logarithm (base e, ln), `log10(x)` is base 10 logarithm
- Note: trig functions use radians (not degrees)

## Variables and naming

## Data types

## Operators

## Conditionals

## Loops

## Lists

Revised Fall 2026 SNR
