<!-- 
  * Develop two assignments that are different types for your unit plan.
  * Describe the assignment, including student facing instructions in a markdown file. Save this file in your own personal work repository.
  * This is individual work, that can be incorperated into your unit plan later. -->
  
  ##  Values and Data Types
  A value is one of the fundamental things: like a letter or a number that a program manipulates. The values that students have seen so far are 2 (the result when we added 1 + 1), and "Hello, World!".

These values belong to different data types: 2 is an integer, and "Hello, World!" is a string, so-called because it contains a string of letters. You (and the interpreter) can identify strings because they are enclosed in quotation marks.

The print statement also works for integers.

<hr>

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


## Definitions and use
In the context of programming, a function is a named sequence of statements that performs a desired operation. This operation is specified in a function definition. In Python, the syntax for a function definition is:

def NAME( LIST OF PARAMETERS ):<br>
     STATEMENTS<br>
You can make up any names you want for the functions you create, except that you can’t use a name that is a Python keyword. The list of parameters specifies what information, if any, you have to provide in order to use the new function.

There can be any number of statements inside the function, but they have to be indented from the def. In the examples in this book, we will use the standard indentation of four spaces. Function definitions are the first of several compound statements we will see, all of which have the same pattern:

A header, which begins with a keyword and ends with a colon.
A body consisting of one or more Python statements, each indented the same amount – 4 spaces is the Python standard – from the header.
In a function definition, the keyword in the header is def, which is followed by the name of the function and a list of parameters enclosed in parentheses. The parameter list may be empty, or it may contain any number of parameters. In either case, the parentheses are required.

The first couple of functions we are going to write have no parameters, so the syntax looks like this:

def new_line():<br>
    print("")          # a print statement with an empty string prints a new line<br>
This function is named new_line. Its body contains only a single statement, which outputs a newline character. (That’s what happens when you use a print command with an empty string.)

Defining a new function does not make the function run. To do that we need a function call. Function calls contain the name of the function being executed followed by a list of values, called arguments, which are assigned to the parameters in the function definition. Our first examples have an empty parameter list, so the function calls do not take any arguments. Notice, however, that the parentheses are required in the function call:

print("First Line.")<br>
new_line()<br>
print("Second Line.")<br>
The output of this program is:<br>

First line.

Second line.<br>
The extra space between the two lines is a result of the new_line() function call. What if we wanted more space between the lines? We could call the same function repeatedly:

print("First Line.")<br>
new_line()<br>
new_line()<br>
new_line()<br>
print("Second Line.")<br>
Or we could write a new function named three_lines that prints three new lines:

def three_lines():<br>
    new_line()<br>
    new_line()<br>
    new_line()<br>

print("First Line.")<br>
three_lines()<br>
print("Second Line.")<br>
This function contains three statements, all of which are indented by four spaces. Since the next statement is not indented, Python knows that it is not part of the function.

You should notice a few things about this program:

You can call the same procedure repeatedly. In fact, it is quite common and useful to do so.
You can have one function call another function; in this case three_lines calls new_line.
So far, it may not be clear why it is worth the trouble to create all of these new functions. Actually, there are a lot of reasons, but this example demonstrates two:

Creating a new function gives you an opportunity to name a group of statements. Functions can simplify a program by hiding a complex computation behind a single command and by using English words in place of arcane code.
Creating a new function can make a program smaller by eliminating repetitive code. For example, a short way to print nine consecutive new lines is to call three_lines three times.
Pulling together the code fragments from the previous section into a program named tryme1.py, the whole program looks like this:

def new_line():<br>
    print("")<br>

def three_lines():<br>
    new_line()<br>
    new_line()<br>
    new_line()<br>

print("First Line.")<br>
three_lines()<br>
print("Second Line.")<br>

This program contains two function definitions: new_line and three_lines. Function definitions get executed just like other statements, but the effect is to create the new function. The statements inside the function do not get executed until the function is called, and the function definition generates no output.

As you might expect, you have to create a function before you can execute it. In other words, the function definition has to be executed before the first time it is called.

