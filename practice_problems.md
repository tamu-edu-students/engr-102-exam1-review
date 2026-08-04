# Exam 1 Practice Problems

The following problems are for practice when studying for Exam 1. It is recommended that you attempt them using pencil and paper (NOT an IDE) like you will for the exam. After attempting a problem, check your solution by typing it into your favorite IDE and debug. 

Partial credit will be available for code writing problems so please comment your code. It is recommended that you write out your algorithm in comments first, then go back and fill it in with code (see the "pyramid" method in Lecture 5). Several problems (multiple choice, true/false, fill in the blank, etc) will be autograded and no partial credit will be available.

During the exam calculators are not allowed, you won't need one anyway. In addition, you may NOT use your phone, the web to search for additional information, your laptop, your book, your notes, lectures on Canvas, or any form of electronic media.

- [Autograded Style Problems](#autograded-style-problems)
- [Code Writing Problems](#code-writing-problems)
- [Short Answer Problems](#short-answer-problems)

## Autograded Style Problems
*Go back and review your quizzes for additional autograded style problems including fill in the blank, multiple choice, multiple answer, and true/false type questions.*

For the following problems, write the output of the code. Don't forget `[]` `{}` and/or `,` as needed. Note that code snippets are intentionally not color coded as your printed exam will also be in black and white.

```
# problem 1
x = 5 / 5
print(x)
```
```
# problem 2
print(7 * 2 ** 3 – 12 * 2 // 7 + 8 % 3)
```
```
# problem 3
from math import *
print("ENGR sqrt(625) * 4 + 2")
```
```
# problem 4
a = 3
b = 2
c = 4
print(a * b + c // c – b)
```
```
# problem 5
x = 4
y = 8
t = x
x = y
y = t
z = x / y
print(z)
```
```
# problem 6
x = 7
y = 8
z = x + y / 4
a = (y – x) * 2
z += a
b = z // 2
c = x * 5
c %= 4
print(c)
```
```
# problem 7
bool(int("3.14"))
```
```
# problem 8
x = "3"
print(bool(2 * x – x))
```
```
# problem 9
x = 1.5
y = 4
print(f"{2 * str(x) + str(y)}")
```
```
# problem 10
x = 5 % 2 == 1 and 5 < 2 + 4
print(x)
```
```
# problem 11
a = 3
b = 5
c = 7
print(a > b or not c == b and c > b)
```
```
# problem 12
a = 2
b = 5
c = True
d = "a"
print(a > b or c and d != "a" or not c)
```
```
# problem 13
a = 10
b = 10
c = 20
d = a > b and b <= c
e = not(((c <= a + b and a == 10) or (b == 10 and c != 10)))
print(d or e)
```
```
# problem 14
a = 10
b = 10
c = 20
d = a < b and b >= c or not c <= a – b and a == 10 or b == 20 and c != 5
print(d)
```
```
# problem 15
a = 5
b = 6
c = 7
d = float(str(a * 2)) > float(str(b + c))
e = float(str(a) * 2) >= float(str(b) + str(c)) – 11
print(d or e)
```
```
# problem 16
a = True
b = bool("False")
c = 5 > 8
d = a and b and c
e = not a or not (b and c)
print(d, e)
```
```
# problem 17
x = "7"
y = "16"
z = 772
if x * 2 + "2" == y:
    print(y + y)
elif x * 2 + "2" == z:
    print(z + z)
else:
    print(x + x)
```
```
# problem 18
a = "Aitor_cruzado"
if "ai" in a:
    b = a[:-8]
elif "cr" in a:
    b = a[9:999]
print(b)
```
```
# problem 19
a = int(False) + 6
b = int("2" * 2) – 48 / 3
z = int("2" + "3")
if a == b:
    z %= 5
elif b == 6:
    z //= 5
else:
    z += 5
```
```
# problem 20
a = 1
b = 2
c = "a"
d = int(float("3.14"))
if a == 1 and d == 3.14:
    print("Green")
elif c == a or d > 3:
    print("Red")
else:
    print("Yellow")
```
```
# problem 21
x = 0
y = 2
if x > 0 and y > 0:
    print("x > 0 and y > 0")
elif x > 0 or y > 0:
    if x > 0:
        print(x)
elif x == 0:
    print(y)
```
```
# problem 22
x = 10
y = 5
if x % 2 == 0:
    if y > 5:
        print("A")
    else:
        print("B")
        print("C")
else:
    if y < 5:
        print("D")
    else:
        print("E")
        print("F")
print("G")
```
```
# problem 23
a = 5
b = "b"
c = True
print("The answer is...", end=" ")
if a != 10:
    print("A", end=" ")
elif b == "b":
    print("B", end=" ")
else:
    print("C", end=" ")
z = c and bool(a)
print(z, end=" ")
d = a ** 3 + 25 % 3 - 12 // 5
print(d)
```
```
# problem 24
mystr = "The quick brown fox jumped over the lazy dog"
print(mystr[:3], end=" ")
if mystr[4] == "q":
    if "fox" in mystr:
        print("fox", end=" ")
    else:
        print("dog", end=" ")
    if mystr[-5] != "z":
        print("jumped", end=" ")
    else:
        print("hopped", end=" ")
elif "x" in mystr:
    if "white" in mystr:
        print("white mouse", end=" ")
    else:
        print("brown cow", end=" ")
    if "y" not in mystr:
        print("sat", end=" ")
    else:
        print("dropped", end=" ")
else:
    print(mystr[4:26], end=" ")
print("down")
```

## Code Writing Problems
stuff

## Short Answer Problems
stuff

Revised Fall 2026 SNR
