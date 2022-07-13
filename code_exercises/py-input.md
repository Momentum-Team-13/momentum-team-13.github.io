---
title: Python Code Break 1
layout: default
nav_exclude: true
---

## Working with input and output

Create a file called `gross_pay.py`. Write your python code in that file.

You should be able to run your program by typing `python gross_pay.py` at your command prompt.

### Exercise 1

Write a program that will ask the user for a number of hours worked and a hourly rate. Calculate the gross pay based off those numbers. Then show the user the total.

```
Enter hours worked: 20
Enter hourly rate: 18.50
Total: $370.0
```

### Exercise 2

Add to the calculation time-and-a-half for hours worked over 40. (*Note: time-and-a-half rate is the hourly rate * 1.5*)

```
Enter hours worked: 55
Enter hourly rate: 20
Total: $1250
```

### Exercise 3

Try to split your program into a function called `calculate_pay(hours_worked, hourly_rate)` and code that takes user input, calls `calculate_pay` and prints out the result.
