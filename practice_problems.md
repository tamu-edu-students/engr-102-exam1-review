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
```
# problem 25
for i in range(1, 4, 2):
    print(i)
```
```
# problem 26
for i in range(4):
    print("Aitor" * i)
```
```
# problem 27
for i in range(12):
    if i % 2 != 1 and i % 3 == 0:
        print(i)
```
```
# problem 28
n = 1
p = "A"
while n < 10:
    p += p
    n += 3
print(n, p)
```
```
# problem 29
x = 4
y = "Gig'em Aggies!"
while x < 100:
    print(x, y)
    x *= x – 2
    y += y
```
```
# problem 30
x = 2
y = "A"
while x < 100:
    print(x, y)
    x *= x
    y += y
```
```
# problem 31
x = 5
mysum = 0
for i in range(4):
    x *= i
    mysum += x
print(x, mysum)
```
```
# problem 32
for i1 in range(1, 3):
    for i2 in range(i1 + 1):
        i1 += 1
        print(f"{i1}{i2}", end=" ")
        i2 += 1
    print()
```
```
# problem 33
mystr = "Howdy! Welcome to Texas A&M Engineering!"
print(mystr[:5] + mystr[6] + mystr[-22:-1] + " students! ")
```
```
# problem 34
a = "Aerospace"
print(a[0])
print(len(a) – 1)
print(len(a) + 0.5 * 3 // 2)
```
```
# problem 35
a = "Aitor"
a[1] = "1"
print(a)
```
```
# problem 36
a = [1, 2, 3, 4, 5, 56, 67]
print(a[7])
```
```
# problem 37
a = "My name is aitor"
count = 0
for i in a:
    if i == "a":
        print(a[:count+7])
        print(count)
    elif i == "i":
        break
    else:
        continue
    count += 1
    print(count)
```
```
# problem 38
mystrs = ["Good Bull", "Whoop", "Hullabaloo", "Howdy", "Gig 'em", "Aggies"]
mynums = [3, 5, 4, 1, 2]
for num in mynums:
    print(mystrs[num], end=" ")
```
```
# problem 39
mylist = []
for i in range(5):
    mylist.append(i ** 2)
print(mylist[-3:])
```
```
# problem 40
a = [1, 34, 3]
b = 2
a.append(b)
a.sort()
print(a)
```
```
# problem 41
AB = 0
V = [9, 5, -3, 6, -1, 0]
for i in range(len(V) – 2):
    if V[i] < 0:
        AB += 1
print("AB =", AB)
```
```
# problem 42
data = [[[1, 2], [3, 4]], [[5, 6], [7, 8]]]
print(data[1][0][0])
```
```
# problem 43
a = [[1, 2, 3, 4], ["a", "b"]]
for i in a:
    print(i)
    print(i[1:100])
```
```
# problem 44
a = [1, 3, 4, 56, 2, 32, 13, 124, 5534]
for i in range(len(a)):
    if a[i] % 2 == 1:
        print(a[i], i, sep=",", end=":")
print()
print(a[-4:])
```
```
# problem 45
a = 3
b = [1, 2, 3, 4, 5]
for i in b:
    for j in a:
        print(i, j, end="")
```
```
# problem 46
a = [12, 89, 45, 12, 67, 3, 4, 9, 20, 34, 45, 67, 199, 67]
count = 0
for i in a:
    if i % 2 == 0:    # What happens if we use i % 5 == 0?
        for j in range(len(a)):
            if i == j:
                continue
            else:
                count += 1
    else:
        count -= 1
print(count)
```
```
# problem 47
a = [12, 89, 45, 12, 67, 3, 4, 9, 20, 34, 45, 67, 199, 67]
count = 0
for i in a:
    if i % 2 == 0:
        for j in range(len(a)):
            if i == j:
                break    # this line is different
            else:
                count += 1
    else:
        count -= 1
print(count)
```
```
# problem 48
a = [12, 89, 45, 12, 67, 3, 4, 9, 20, 34, 45, 67, 199, 67]
count = 0
for i in a:
    if i % 2 == 0:
        for j in range(len(a)):
            if i == a[j]:    # this line is different
                break
            else:
                count += 1
    else:
        count -= 1
print(count)
```
```
# problem 49
a = [12, 89, 45, 12, 67, 3, 4, 9, 20, 34, 45, 67, 199, 67]
count = 0
for i in a:
    if i % 5 == 0:    # this line is different
        for j in range(len(a)):
            if i == a[j]:
                print(i, end=", ")
                continue    # these 2 lines are different
            else:
                count += 1
    else:
        count -= 1
print(count)
```
Problem 50<br>
Which of the following are valid variable names in Python? Choose all that apply.
- `10_kilos`
- `mass-kg_`
- `_10_KG_Mass`
- `ma$$`

Problem 51<br>
Will the code below run without an error? If not, find and correct the error.
```
side = input("Please enter the side of a square: ")
a = side ** 2
print(f"The area of the square is: {a}")
```

Problem 52<br>
Starting with the following line of code, write one more line of code that will calculate the radius of a circle with area equal to 6.5 cm^2 and display the result to the console, including a text description.
```
from math import *
<your code goes here>
```

Problem 53<br>
What is the data type of the variable `x` after the following line of code is executed?<br>
`x = str(int("5 + 6"))`
- Integer
- Floating-point number
- Boolean
- String
- The code contains an error

Problem 54<br>
What is the data type of the variable `x` after the following line of code is executed?<br>
`x = int(float("97.9"))`
- Integer
- Floating-point number
- Boolean
- String
- The code contains an error

Problem 55<br>
Given x = 3 and y = 5, evaluate the following Boolean expressions:<br>
- `x != y – 2`
- `x >= 0 and not x < 10`
- `x < 0 and x < 10`
- `x >= 0 and x < 2`
- `x < 0 or y < 5`
- `not x > 0 or x < 10`

Problem 56<br>
Which code snippet below correctly finds the number of digits of the sum of two integers? Either value may be positive, negative, or zero.

Examples:
- 12 + 6 = 18 → 2 digits
- -12 + 2 = -10 → 2 digits (the negative sign does not count)
- 0 + 3 = 3 → 1 digit

The following code is executed before each answer below:
```
num1 = int(input("Enter first integer: "))
num2 = int(input("Enter second integer: "))
numSum = num1 + num2
```

Answer choices:
```
# answer A
myString = str(numSum)
strLength = len(myString) – 1
print(f"number of digits of {numSum} is {strLength}")
```
```
# answer B
count = 0 
temp = abs(numSum) 
while temp > 1: 
    temp = temp / 10 
    count = count + 1 
print(f"number of digits of {numSum} is {count}")
```
```
# answer C
if numSum < 0: 
    myString = str(-numSum) 
else: 
    myString = str(numSum) 
strLength = len(myString) 
print(f"number of digits of {numSum} is {strLength}")
```
D.	None of the above


## Code Writing Problems
stuff

## Short Answer Problems
stuff

Revised Fall 2026 SNR
