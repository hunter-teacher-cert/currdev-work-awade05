<!-- 
  * Develop two assignments that are different types for your unit plan.
  * Describe the assignment, including student facing instructions in a markdown file. Save this file in your own personal work repository.
  * This is individual work, that can be incorperated into your unit plan later. -->
  
  ##  Values and data types
  A value is one of the fundamental things: like a letter or a number that a program manipulates. The values that students have seen so far are 2 (the result when we added 1 + 1), and "Hello, World!".

These values belong to different data types: 2 is an integer, and "Hello, World!" is a string, so-called because it contains a string of letters. You (and the interpreter) can identify strings because they are enclosed in quotation marks.

The print statement also works for integers.

### Converting between types.
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




