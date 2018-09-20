
# Python for Everyone

![python_icon](https://www.python.org/static/community_logos/python-logo-master-v3-TM.png)

## Exercise 1.13

1\. What is the function of the secondary memory in a computer

   b) Store information for the long term, even beyond a power cycle.

----

2\. What is a program?

   A sequence of statements that have been crafted to do something.

----

3\. What is the difference between a compiler and an interpreter?

   It is the nature of an *interpreter* to be able to have an **interactive conversation**/use high-level language.
   
   A *compiler* needs to be **handed the entire program in a file**, and then it runs a process to translate the high- level source code into machine language and then the compiler puts the resulting machine language into a file for   later excution.

----

4\. Which of the following contains "machine code"?

   c) The python interpreter

----

5\. What is wrong with the following code?

   The function name "print" is misspelled as "primt"

----

6\. Where in the computer is a variable such as "X" stored after the following Python line finishes?

    ```python
    x = 123
    ```
   b) Main memory. The value of the variable is not stored and not avaliable for retreval after the program quites.

----

7.\ What will the following program print out?

    ```python
    x = 43
    x = x + 1
    print(x)
    ```
   b) 44

----

8\. Explain each of the following using an example of a human capability.

    1) Central processing unit: brain
    2) Main memory: waking consciousness
    3) Secondary memory: long-term memory
    4) Input device: ear, eye, nose
    5) Output device: mouth

----

9\. How to you fix a "Syntax Error?"

   Correct the grammar and the spelling in the source code so the program can understand the instruction.

## Exercise 2.15

2\. Write a program that uses `input` to prompt a user for their name and then welcome them.


```python
name = input("May I ask your name?")
print("Welcome to the Wonderland", name, sep=", ", end="!")
```

----
3\. Write a program to prompt the user for hours and rate per hour to compute gross pay.


```python
hour = int(input("How much hours do you work?"))
rate = int(input("What is the rate per hour?"))
gross_pay = print("The gross pay is $", hour * rate, sep = "", end = ".")
```

----
4\. Write a program which prompts the user for a Celsius temperature, convert the temperature to Fahrenheit, and print out the converted temperature.


```python
celsius_temp = int(input("The Celsius temprature:"))
fahrenheit_temp = celsius_temp * 1.8 + 32
print("The Fahrenheit temperature is", fahrenheit_temp, end = "°F.")
```

    The Celsius temprature:10
    The Fahrenheit temperature is 50.0°F.

# Exercise 3.11

1\. Rewrite your pay computation to give the employee 1.5 times the hourly rate for hours worked above 40 hours.


```python
hour = int(input("How much hours do your work?"))
rate = int(input("What's your rate?"))

if hour >= 40:
    payment = hour * rate * 1.5
else:
    payment = hour * rate * 1.5

print("The gross pay is $", payment, sep = "", end = ".")
```

----
2\. Rewrite your pay program using `try` and `except` so that your program handles non-numeric input gracefully by printing a message and exiting the program.

----
3\. Write a program to prompt for a score between 0.0 and 1.0. If the score is out of range, print an error message. If the score is between 0.0 and 1.0, print a grade using the following table:

| Score         | Grade         |
| ------------- |:-------------:|
| >= 0.9        | A             |
| >= 0.8        | B             |
| >= 0.7        | C             |
| >= 0.6        | D             |
| < 0.6         | F             |
