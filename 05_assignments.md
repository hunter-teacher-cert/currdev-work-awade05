<!-- 
  * Develop two assignments that are different types for your unit plan.
  * Describe the assignment, including student facing instructions in a markdown file. Save this file in your own personal work repository.
  * This is individual work, that can be incorperated into your unit plan later. -->
  
  ##  Values and Data Types
  A value is one of the fundamental things: like a letter or a number that a program manipulates. The values that students have seen so far are 2 (the result when we added 1 + 1), and "Hello, World!".

These values belong to different data types: 2 is an integer, and "Hello, World!" is a string, so-called because it contains a string of letters. You (and the interpreter) can identify strings because they are enclosed in quotation marks.

The print statement also works for integers.


#### Converting between types.
Sometimes you may find it helpful or necessary to change a value of one type to another type. For example the value "3" is a string because it enclosed in quotes. But the contents of the string, the character 3 is also a valid integer. You can convert a value to an integer using the int() built in function. 

Try these examples in the python shell:
> int("7")
> int(3.2)
> int("3.2")
> int(5.7)
> int("puppy")
> ans="12"
> int(ans)

The print statement also works for integers.

> print(4)

If you are not sure what type a value has, the interpreter can tell you.

> type("Hello, World!")

Double quoted strings can contain single quotes inside them, as in "Bruce's beard", and single quoted strings can have double quotes inside them, as in 'The knights who say "Ni!"'.

When you type a large integer, you might be tempted to use commas between groups of three digits, as in 1,000,000. This is not a legal integer in Python, but it is legal:

> print(1,000,000)

Students will experiment with these different types of Data Types to learn the difference. 

<hr>

## Working with Strings and Data Types

The goals for this assignment are:

- Manipulate Python numeric and string data types

- Learn to apply the accumulator pattern to numeric and string types to solve problems

- Learn to iterate over data using for loops

- Practice string operations +, len(), []

1. Farmers' Market
A vendor at a local farmers' market wants a program to tally sales of apples over the harvest season. Write a program called market.py that computes the total sales over a number of days entered by the user. The program should prompt the user for the number of bushels of apples sold per day and the price per bushel each day. Before exiting, the program should print the total number of bushels sold and the total amount of sales in dollars.

Two examples of the running program are shown below. User input is shown in bold.

```
$ python3 market.py
Enter number of sales days: 2

Enter number of bushels sold: 3.5
Enter price per bushel: 24

Enter number of bushels sold: 2
Enter price per bushel: 22.50

Total bushels sold: 5.5
Total sales: $129.0

$ python3 market.py
Enter number of sales days: 3

Enter number of bushels sold: 1
Enter price per bushel: 20

Enter number of bushels sold: 1
Enter price per bushel: 20

Enter number of bushels sold: 1
Enter price per bushel: 20

Total bushels sold: 3.0
Total sales: $60.0

```
2. Text Slant

Write a program called txtslant.py that prompts the user for a string, and then prints one character of the string per line in a diagonal pattern as shown below.

```
$ python3 txtslant.py
Enter a phrase: weee!
w
 e
  e
   e
    !

$ python3 txtslant.py
Enter a phrase: autumnal equinox
a
 u
  t
   u
    m
     n
      a
       l

         e
          q
           u
            i
             n
              o
               x
               
```
3. Text Weave

Write a program called txtweave.py that prompts the user for a string msg, and then prints out a new string consisting of the characters in msg in forward and reverse interleaved. For example, if the user enters the string hello, you would take the letters in the original order:

```
h e l l o
```

and reverse order
```
 o l l e h
 ```
 
and interleave them to form the final string
```
hoelllleoh
```
Some examples of the running program are shown below. User input is shown in bold.

```
$ python3 txtweave.py
Enter a phrase: cs21

Text weave is:
c1s22s1c

$ python3 txtweave.py
Enter a phrase: swarthmore
Text weave is:
sewraormthhtmroarwes
```

4. Text Grid

Write a program called txtgrid.py that makes a grid pattern out of strings using + and - symbols. Your program should prompt the user for the number of rows and columns in the grid and the width of all the columns. Each column should consist of width number of - symbols and adjacent columns should be seperated by a +. To design your program figure out how to build a single string that represents a single row in the grid. Then print that string out for the specified number of rows.

Some examples of the running program are shown below. User input is shown in bold.
```
$ python3 txtgrid.py
Enter number of columns: 3

Enter width of column: 2
Enter number of rows: 4

+--+--+--+
+--+--+--+
+--+--+--+
+--+--+--+

$ python3 txtgrid.py
Enter number of columns: 4
Enter width of column: 8
Enter number of rows: 5

+--------+--------+--------+--------+
+--------+--------+--------+--------+
+--------+--------+--------+--------+
+--------+--------+--------+--------+
+--------+--------+--------+--------+
```

