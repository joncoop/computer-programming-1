# The Interactive Shell

At its core, a computer program is a set of instructions that a computer executes to perform a task. In this lesson, we won't make full programs, but we will experiment with some of the types of instructions that can be executed in a Python program. Start the application IDLE in the Python folder. When IDLE starts, the window that opens is the Python shell. At the prompt, we can type in Python statements and see the output immediately.

It is going to be very tempting to copy/paste from the document into IDLE. Don’t! You will learn much more and notice the details of the Python language if you actually type each statement yourself.

## Python as a calculator

The simplest statements that Python can execute are arithmetic expressions. Try typing each of these lines into the shell.

    >>> 3 + 4
    >>> 5 - 9
    >>> 5 * 7
    >>> 37 / 5

These operations probably worked exactly as you expected. There are more operations that Python can evaluate. Use the shell to evaluate the following expressions.

    >>> 2 ** 5
    >>> 37 // 5
    >>> 37 % 5

What is does the ** operator do? If you’re not sure, try using the ** operator with different operands until you figure it out.

Experiment with other operands to determine the rounding rules used by the // operator. What is the rounding rule ? What specific calculations helped you determine this?

What did the % operator do? Keep experimenting with other operands until you figure it out.

## Variables

Enter these statements:

    >>> x = 5
    >>> y = 3

Notice how there was no output this time. Instead, the numbers 5 and 3 were stored in the computer’s memory. Think of x and y as containers holding the values until we want to do something with them later. Since we can also change the values stored in those locations, x and y are called variables.

Now that the values are stored in memory we can perform operations with them. Try…

    >>> x + y
    >>> y / x
    >>> x = 100
    >>> x + y
    >>> x = x + 5
    >>> x
    >>> x = x + 5
    >>> x

Did you get the results you expected from each expression? If not, look through them again until you understand.

## Variables names

In the above examples, we used single letter names for our variables. Variable names don’t need to be single letters like you typically use in math class. Usually it is helpful to give the variables names that represent the information they are storing. Also, you should get in the habit of using only lowercase letters in variable names. For example,

    >>> age = 45

## Strings

Variables can store more than just numbers. If you want to store a sequence of letters and other symbols then you need to use quotations. The value in quotations is called a string.

    >>> name = "Jon Cooper"

You may want to use variable names with more than one word. In Python the convention is to use an underscore to separate words. You cannot have spaces in variable names. There are some other rules for variable names, however if you just remember to use only lowercase letters and underscores you’ll be fine. Store your first and last names as follows:

    >>> first_name = "Jon"
    >>> last_name = "Cooper"

What happens if you try to store your name without using quotes?

What if you store a numeric value in quotes and then try to add it to another number? Write what you tried and the result?

If you want to display more than one value, you can separate them with a + operator. This is called concatenation.

    >>> "My name is" + first_name

Write a statement that makes a variable called `food` that stores the name of your favorite food.
Now write a statement that prints the sentence "[first_name] likes [food]". (Don’t print the brackets. Print the contents of the variables name and food.)

The above statements worked because both "My name is" and the contents of the variables name and food are strings. The variable age is numeric. Try typing the following statement.

    >>> first_name + " is " + age + " years old."

What error message to you get after typing the above statement?

An error occurs because the + operator actually has two meanings in Python. When it occurs between numeric values, the Python interpreter knows to do addition. If it occurs between two strings, then it concatenates them. But if you put a + between a string and a number, then the interpreter doesn’t know what to do. We can fix this by forcing the interpreter to treat the variable age as a string as follows:

    >>> first_name + " is " + str(age) + " years old."

Write a statement that prints the sentence "[first_name] [last_name] is [age] years old and likes [food]". (Don’t print the brackets. Print the contents of the name, age, and food variables. Be sure that a space occurs between your first and last names.)

## Closing the shell

If we close shell now, everything we typed is wiped from memory. But what if we want to execute the same instructions later, perhaps tomorrow or next week? Then we need to write a Python program. That’s the next lesson.
