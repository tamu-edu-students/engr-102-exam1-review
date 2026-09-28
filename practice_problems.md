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
print(z)
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
    else:
        print(y)
elif x == 0:
    print("x == 0")
else:
    print(x + y)
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
a = "3"
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
Write the data type and value of the following code:<br>
`str(float(str(3 / 2) + str(int(3 / 2)))) * int(int(str(2) + str(7)) / int(10.3))`

Problem 56<br>
Given x = 3 and y = 5, evaluate the following Boolean expressions:<br>
- `x != y – 2`
- `x >= 0 and not x < 10`
- `x < 0 and x < 10`
- `x >= 0 and x < 2`
- `x < 0 or y < 5`
- `not x > 0 or x < 10`

Problem 57<br>
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
1.	Write a Python program to take as input 5 birthdays from 5 users (1 each) and output them in chronological order. Dates should be entered with the month and day (not year) in the format "June 6" as a single input per user. You may format the output however you like (including using numbers for the month instead of words). This is a good problem to practice using lists of lists.

Example output:
```
User 1 please enter a birthday: December 12
User 2 please enter a birthday: January 15
User 3 please enter a birthday: April 12
User 4 please enter a birthday: November 25
User 5 please enter a birthday: April 1
------------------------------------------------
January 15
April 1
April 12
November 25
December 12
```

2.	Write a Python program to play a simplified version of the game hangman. Have User 1 input a secret word with a minimum length of 6. Then, take as input from User 2 one letter at a time until they guess a letter that is not in the secret word. At the end of the program, print out the number of guesses and the secret word.

Example output:
```
Enter the secret word: programming
Guess a letter: n
Guess another letter: a
Guess another letter: e
The secret word is: "programming". You took 3 guesses!
```

3.	Write a Python program to take as input from the user a student's UIN. If the UIN exists in the list `roster`, have your program output the first and last name of the student, their major, and their GPA. The list `roster` is a list of lists and you may assume that it is already available in the code. An example of its data is shown below.
```
roster = [["123004567", ["Joe", "Aggie", "ENGE", 3.50]],
          ["123004568", ["Jake", "Green", "OCEN", 3.75]],
          ["123004569", ["Jill", "Apple", "ENGR", 3.25]]]
```
Example output for input `123004567`:
```
Enter a UIN: 123004567
Joe Aggie: ENGE, 3.50
```

4.	Write a Python program that prints out the sum of the even numbers between 2 to 200, inclusive. You must use a loop.

5.	Write a Python program to generate the following patterns exactly as shown **using a single loop** for each pattern.
```
a
bb
ccc
dddd
eeeee
```
```
>
>>
>>>
>>
>
```
```
***
**
*
**
***
```
```
ooooo
 oooo
  ooo
   oo
    o
```
```
xxxx
xxxo
xxoo
xooo
oooo
```

6.	Write a Python program that will repeatedly ask a user to input a person's age. The program should continue to ask for input until a negative number is entered, indicating that the user is done inputting data. Assume at least one valid value is entered before a negative number. The program should determine the total number of people and the minimum and maximum ages entered. Do not include the negative number in your calculations. The results should be printed to the screen using the format shown below. Include the header and align the columns.

Example output:
```
Enter an age: 17
Enter another age: 24
...
Enter another age: -1
Number of people  Minimum age  Maximum age
32                17           24         
```

7.	A schematic for converting phone letters to digits mapping is shown in the image below. Write a Python program that prompts the user to enter a 10-character phone number in this format `XXX-XXXXXXX`. Your program should replace the last seven alphabetic characters by their equivalent digits and display the entered phone number in this format `XXX-XXX-XXXX`. For example, if the user enters `800-GOFEDEX`, your program output would convert the number to `800-463-3339`. You may assume that the last seven characters are alphabetic characters from A to Z.

![New #ios6 dial pad design | Jakob Montrasio | Flickr](exam1_practice_prob_7.jpg)

Example output for input `800-GOFEDEX`:
```
Enter a phone number in this format XXX-XXXXXXX: 800-GOFEDEX
800-GOFEDEX is equivalent to 800-463-3339
```

8.	Write a Python program that takes in an integer between one hundred and one million, inclusive. You may assume the user always enters an integer. If the user enters a value outside the interval, print an error message. For any valid input, check the last two digits in the number: if both are even, print their sum; if both are odd, print their product. Otherwise, print `One odd, one even!`

You may use the built-in `len()` function. Do **NOT** use loops, lists/tuples, or the `sort()` and `sorted()` functions, or any of the string class methods. Use good coding practices.

Example output using input values `15`, `157`, `3468`, and `12345`:
```
Enter an integer between 100 and 1000000, inclusive: 15 
Wrong input!
```
```
Enter an integer between 100 and 1000000, inclusive: 157 
Both odd! 
Product = 35
```
```
Enter an integer between 100 and 1000000, inclusive: 3468 
Both even! 
Sum = 14
```
```
Enter an integer between 100 and 1000000, inclusive: 12345 
One odd, one even!
```

9.	Write a Python program that takes as input a value of `n` (`n` is a positive integer) and then calculates and prints the sum of `n + nn + nnn`. For example, if `n = 12`, the sum is `12 + 1212 + 121212 = 122436`; if `n = 1`, the sum is `1 + 11 + 111 = 123`; if `n = 345`, the sum is `345 + 345345 + 345345345 = 345691035`.

Example output using input values `1`, `12`, and `345`:
```
Enter an integer: 1
1 + 11 + 111 = 123
```
```
Enter an integer: 12
12 + 1212 + 121212 = 122436
```
```
Enter an integer: 345
345 + 345345 + 345345345 = 345691035
```

10.	Write a Python program that takes as input a word or sentence and prints the reverse. You MUST use a for loop.

Example output for input `howdy all!`:
```
Enter some text: howdy all!
Reversed: !lla ydwoh
```

11.	Write a Python program to print the table shown below. For each integer `n` between 2 and 5 (inclusive), print the numbers between `n` and `n * 10` that are multiples of `n`. You MUST use nested loops.

Example output:
```
----------------------------------------------- 
Integer Multiples 
----------------------------------------------- 
2       2, 4, 6, 8, 10, 12, 14, 16, 18, 20 
3       3, 6, 9, 12, 15, 18, 21, 24, 27, 30 
4       4, 8, 12, 16, 20, 24, 28, 32, 36, 40 
5       5, 10, 15, 20, 25, 30, 35, 40, 45, 50
-----------------------------------------------
```

12.	Write a Python program that takes as input a positive integer then adds and prints all of the digits in the number.

Example output for input values `12` and `8675309`:
```
Enter a positive integer: 12
Sum of the digits: 3
```
```
Enter a positive integer: 8675309
Sum of the digits: 38
```

13.	Write a Python program that takes as input a positive integer that contains at least 10 digits, and a single digit. Have your program remove all occurrences of the specified digit from the initial number and print the result. 

Example output for input values `3479734103487314` and `3`:
```
Enter an integer with 10+ digits: 3479734103487314
Enter a digit: 3
New number is 479741048714
```

14.	Write a Python program that takes as input 5 items that are sold in a school cafeteria (name and cost). Then take as input the amount of money that the user has. Print all of the items that the user can afford to buy.

Example output:
```
Enter 5 items and their cost
Item 1: apple 0.50
Item 2: banana 0.50
Item 3: milk 1.00
Item 4: pizza 5.00
Item 5: hot dog 3.00
How much money do you have? 2.00
You can afford apple, banana, or milk
```

15.	Write a Python program that takes as input a positive integer and then prints all members of the [Fibonacci sequence](https://en.wikipedia.org/wiki/Fibonacci_sequence) up to that number (inclusive).

Example output for input `102`:
```
Enter a positive integer: 102
Here is the Fibonacci sequence up to 102:
0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89
```
Now write a Python program that takes as input a positive integer `n` and then prints the first `n` members of the Fibonacci sequence.

Example output for input `8`:
```
Enter a positive integer: 8
Here are the first 8 members of the Fibonacci sequence:
0, 1, 1, 2, 3, 5, 8, 13
```

16.	Write a Python program that takes as input the number of rows and columns of a 2D `m×n` matrix, and prints a list of lists of that matrix. The values of the matrix are the sum of the row and column indices, where indices start at zero. Do NOT use `numpy` or `sympy`. You MUST use a loop.

Example output for input values `3` and `4`:
```
Enter the number of rows: 3
Enter the number of columns: 4
[[ 0, 1, 2, 3], [1, 2, 3, 4], [2, 3, 4, 5]]
```

17.	Write a Python program that takes as input a list of numeric values then outputs the second largest value. You may assume that all values are unique. As a challenge, do NOT use the `max()`, `min()`, or `sort()` functions.

Example output:
```
Enter some numbers: 1.2 3.4 5.6 7.8 123.456 102 8 6 7 5 3 0 9 -987.6
The second largest value is 102.0
```

18.	Write a Python program that will ask the user to input words until the user inputs `stop`, `Stop`, `STOP`, `StOp`, etc. You may assume that all words start with different letters. Have your program print the number of words inputted by the user and the first word if they were arranged in alphabetical order. You may NOT use containers such as lists, dictionaries, sets, or tuples. 

Example output:
```
Enter a word: dog
Enter another word: howdy
Enter another word: cat
Enter another word: five
Enter another word: red
Enter another word: stoP
If these 5 words were to be sorted alphabetically, the first word would be "cat"
```

19.	Write a Python program that asks the user to input 5 integers, all on one line, with a single space in between. The program should check to see if any of the 5 numbers are duplicates of another (i.e. check whether any of the integers were entered more than once.)  If a duplicate is found, the program should print `Duplicates`, otherwise it should print `All Unique`.

Example output for input `1 2 3 3 5`:
```
Enter five integers: 1 2 3 3 5
Duplicates
```

Example output for input `1 2 3 4 5`:
```
Enter five integers: 1 2 3 4 5
All Unique
```

20.	Write a Python program that will ask the user to input two integers and calculate the sum of the integers between the inputted numbers (inclusive) that are multiples of 4. If the user enters a second integer that is smaller than the first, print a message and do no calculations. Do NOT use containers such as lists, tuples, dictionaries, or sets.

Example output for inputs `2` and `12`:
```
Enter integer 1: 2
Enter integer 2: 12
The sum of multiples of 4 between 2 and 12 is: 24
```

21.	Write a Python program that will repeatedly ask a user to enter names and ages of people, stopping when an age of 0 is entered (and not processing that person).  The program should collect this information, and then output the average age, the name of the oldest person, and the name of the youngest person. You may assume no two people have the same age.

Example output:
```
Enter the name and age of the next person: Ritchey 39
Enter the name and age of the next person: Zoe 6
...
Enter the name and age of the next person: Nobody 0
The average age is 21.3
Frank is the oldest at 85
Ada is the youngest at 3
```

22.	Write a Python program that takes as input positive numbers until a negative value is entered. The program should then output the maximum number, the minimum number, and the average value. Do NOT use containers such as lists, tuples, dictionaries, or sets.

Example output:
```
Enter a number: 1.1
...
Enter a number: -12
Maximum: 102.0, Minimum: 0.12, Average: 20.25
```

23.	Write a Python program that asks the user for an area, then prints out the radius of a circle with that area, and the length of one side of a square with the same area. Format your output to display one decimal place.

Example output for input `5`:
```
Enter an area: 5
A circle with area 5.0 has radius: 1.3
A square with area 5.0 has side length: 2.2
```

24.	Write a Python program that allows the user to enter two (2) integers and then prints all of the values between (and including) the starting and ending integers, that are multiples of both 5 and 7.  Format your output nicely with a comma and space between each number.

Example output for inputs `240` and `385`:
```
Enter the first integer: 240
Enter the second integer: 385
Multiples: 245, 280, 315, 350, 385
```

25.	Given a list of words stored in the variable `list_words`, write a Python program to print the longest word in the list and its length. You may assume that there is only one word of the longest length in the list.

Example output:
```
The longest word "antidisestablishmentarianism" has 28 characters
```

26.	Write a Python program that takes as input a sentence and prints the sentence with every word reversed.

Example output for input `a man a plan a canal panama`:
```
Enter a sentence: a man a plan a canal panama
Words reversed: a nam a nalp a lanac amanap
```

27.	The series expansion for $\ln⁡ \left( \frac{1+x}{1-x} \right)$ on the interval $-1<x<1$ is as follows:

$$\sum_{n=1}^{\infty}\frac{2}{2n-1}x^{2n-1}=2x+\frac{2}{3}x^3+\frac{2}{5}x^5+\frac{2}{7}x^7+...$$

Write a Python program that takes as input a value of $x$ on the interval $-1<x<1$. Have your program check that $x$ is within the specified interval, and continue to prompt the user to enter a value until it is. Then compute an approximation for $\ln⁡ \left( \frac{1+x}{1-x} \right)$ using the series expansion summation above. Continue the summation until the absolute value of the term to be added is less than $10^{-6}$. For example, if $x=0.5$ the first term for $n=1$ is $\frac{2}{2 \ast 1-1} 0.5^{2 \ast 1-1}$ or 1. Since this term is greater than $10^{-6}$, add the term to the summation and continue. Eventually one of the terms will be less than $10^{-6}$, and the summation stops and prints the result. **Note:** [Check out this page](https://github.com/tamu-edu-students/engr-102-lab-6-team/blob/main/more_on_sums.md) for an explanation of calculating series and summation using loops.

Example output for input `0.5`:
```
Enter a value for x: 0.5
ln((1+x)/(1-x)) is approximately 1.098611131435838
```

28.	The Maclaurin series expansion for $\frac{1}{1-x}$ on the interval $-1<x<1$ is as follows:

$$\sum_{n=0}^{\infty}x^n=1+x+x^2+x^3+x^4+...+x^n$$

Write a Python program that takes as input a value of $x$ on the interval $-1<x<1$ then computes an approximation for $\frac{1}{1-x}$ using the series expansion summation above. The summation should continue until the term to be added is less than $10^{-6}$ in absolute value. Hint: Note that each term in the series is $x$ raised to a power, including the first two terms: $x^0=1$ and $x^1=x$. **Note:** [Check out this page](https://github.com/tamu-edu-students/engr-102-lab-6-team/blob/main/more_on_sums.md) for an explanation of calculating series and summation using loops.

Example output for input `0.5`:
```
Enter a value for x: 0.5
1/(1-0.5) is approximately 1.9999980926513672
```

29.	Given a list `xdata` of arbitrary length that contains values of $x$, write a Python program to calculate a $y$ value for each $x$ value using the equation below. Store the calculated $y$ values in a list named `ydata`. Do NOT use `numpy` or `sympy`. Use list functions, methods, and operators.
$$y=4.12x^2+1.52x-7.1$$

30.	Sheldon Cooper's (of Big Bang Theory) favorite number is 73. One of the reasons is that 73 is a prime number and there are 21 prime numbers between 1 and 73. A prime number is an integer greater than 1 that is not divisible by another integer other than 1 (the only even number that is a prime number is 2; all other prime numbers are odd). Write a Python program to calculate and print the prime numbers between 1 and 73 (but not including 73). Your program will also need to count the prime numbers to see if this is really the 21st prime number.

31.	Write a Python program that takes as input an arbitrary number of masses and corresponding volumes then calculates and prints the density for each pair.

Example output:
```
Enter the masses: 10 22.5 30
Enter the volumes: 5 2 1.5
The densities are: 2.0, 11.25, 20.0
```

32.	Write a Python program that takes as input from the user a 4-digit combination, where each digit is between 0 and 9. Represent the four wheels of the lock using a list of lists, where each inner list contains the possible digits 0 through 9 for one wheel. Your program should systematically try possible combinations until it finds the combination entered by the user. When the correct combination is found, print the combination and the number of attempts required. Assume the combination may contain repeated digits. A combination such as `0042` should be treated as a valid four-digit combination. Hint: Take in the combination as a string to preserve leading zeros.

Example Output
```
Enter a 4-digit combination: 0042
Combination found: 0042
```

Now add to your code to output the number of attempts to find the combination. This value will depend on your solution method to try different combinations.

33.	Write a Python program that takes as input the radius of a circle then calculates and prints the items below. Print the values using two decimal places.
- The area and perimeter (circumference) of the circle
- The side length of a square with the same area as the circle
- The side length of a square with the same perimeter as the circle

Example output for input `1.0`:
```
Enter the radius: 1.0
The circle has area 3.14 and perimeter 6.28
A square with equal area has side length 1.77
A square with equal perimeter has side length 1.57
```


## Short Answer Problems
You won't have problems like this on the exam, but they are great for studying!

1.	What are the differences in the following mathematical operators? `/`, `%`, `//`

2.	How do you format your output to display a number with exactly 3 decimal places?

3.	What are the different assignment operators? Provide an example for each.

4.	List all of the data types we have used in this class so far and provide an example for each. How do you convert between data types?

5.	Briefly explain when it is a good idea to use an `if-elif-else` statement instead of multiple `if` statements. When is it a good idea to nest `if` statements?

6.	Name 3 good reasons for including comments when programming.

7.	Briefly explain why it is bad practice to use the "arch" method of program development. Briefly explain the "pyramid" approach to program development.

8.	What is "debugging"?

9.	Briefly explain when it is best to use a `for` loop vs a `while` loop.

10.	What are the similarities between strings and lists?

11.	Given the string below, write one line of code to convert it into a list of its words.<br>
`mystr = "Aggie Engineers Rock And Are In High Demand By Industry"`

12.	Given a list `L` of length greater than 10, write the code to create a new list `L_new` containing the 4th through 7th elements of `L`. Next write the code to remove the 2nd, 3rd, and 4th elements of `L`. Next write code to insert a new value as the 2nd element of `L`. 

13.	Please review all lecture examples and quizzes.

14.	Please review examples and activities in your textbook and resources posted on Canvas.

15.	Please review optional labs for more coding practice.


Revised Fall 2026 SNR
