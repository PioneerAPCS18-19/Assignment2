# Assignment 2

**Remember to put your name at the top of your file.**

A convenient algorithm for determining the date of Easter in a given year was devised in 1876 and first appeared in Butcher’s Ecclesiastical Handbook. This algorithm holds for any year in the Gregorian calendar, which means years including and after 1583. Subject to minor adaptations, the algorithm is as follows:

1. Let y be the year (such as 1583 or 2003).
2. Divide y by 19 and call the remainder a. Ignore the quotient.
3. Divide y by 100 and get a quotient b and a remainder c.
4. Divide b by 4 and get a quotient d and a remainder e.
5. Divide b + 8 by 25 and get a quotient f. Ignore the remainder.
6. Divide b - f + 1 by 3 and get a quotient g. Ignore the remainder.
7. Divide 19 \* a + b - d - g + 15 by 30 and get a remainder h. Ignore the quotient.
8. Divide c by 4 and get a quotient i and a remainder k.
9. Divide 32 + 2 \* e + 2 \* i - h - k by 7 and get a remainder r. Ignore the quotient.
10. Divide a + 11 \* h + 22 \* r by 451 and get a quotient m. Ignore the remainder.
11. Divide h + r - 7 \* m + 114 by 31 and get a quotient n and a remainder p.

The month is n and the day is p+1

**Write a program to solve for the day that Easter falls on for a given year.**

**Your program should have a variable for the desired year, display the values for all of the variables,
and output the date for Easter.**

**Your code will be graded on both functionality and proper style (indentation, variable names, readability, etc.).**

Here is a sample output for 2020.

```
a: 6

b: 20

c: 20

d: 5

e: 0

f: 1

g: 6

h: 18

i: 5

k: 0

r: 3

m: 0

n: 4

p: 11

Easter is on 4/12 in 2020
```

Verify that the program gives the correct date of Easter for the current year.

