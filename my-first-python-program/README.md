# My First Python Program

Until now, we have been typing Python statements one at a time into the interactive shell. This has given us the opportunity to experiment with Python statements and see the output. Being limited to entering and executing statements one at a time is limiting, however. First, we really can’t write Python instructions to solve complex tasks. More limiting is the fact that once we close the shell, all of our work is gone forever. So let’s write our first program.

The Interactive DeveLopment Environment we have been using to write Python code is called IDLE. Thus far, we have only used the interactive shell, but IDLE has another part called the file editor. This is where we can write and more importantly, save Python code.

To start the file editor, click the File menu from within the interactive shell. Then select "New File". A blank window will appear for you to type your program. Enter the following code. Remember, you should actually type it all yourself. Don’t just copy/paste.

    # This program says hello and greets a person by name.
    #
    # Your Name
    # August 20, 2019

    print("Hello.")
    print("What is your name?")
    name = input()
    print("It is good to meet you, " + name + ".")

Before running the program, we must save the file. Go back to the File menu and select Save As…. Give the file the name "hello.py" and save it to a folder called "my-first-python-programs". Now go to the Run menu and select Run Module to see your program run.

When the program runs, each line of code is executed sequentially until the end is reached. Let’s go through the code and see what each line does.

## Comments

Lines 1-4 begin with a # sign (pound sign, or as you kids like to say a 'hashtag'). Comments are not included in the program for the computer. In fact, they are ignored when you run the program. Instead, they are used to remind the programmer what they are trying to do or to help others that might look at your code.

Throughout this course, we’ll use comments at the head of each program to indicate the purpose of the program and to give ourselves credit for the work.

## Printing

Python has many built-in functions that we can use. One is the `print` function. The print function takes the string inside the parentheses and displays it on the screen. In

The first two print statements display a greeting to the user and ask for the person’s name. The last call to the print function uses the + operator to concatenate the string "It is good to meet you" with the person's name.

If you want to display a blank line in your output, you can use the print function without anything in the parentheses like this `print()`.

## Input

The `input` function pauses the program and waits for the user to enter text. It usually doesn’t make sense to ask for input unless you store the data somewhere, so in this program the text entered is stored in the `name` variable.

## Ending the program

Once the final statement is executed, the program terminates. All of the information stored in variables is forgotten by the computer. You can however run the program as many times as you like, and enter a different name every time.

## Questions

- How does the appearance of comments differ from other code when viewed in the file editor? Of functions? Of variables? Of strings in quotes?
- What is the file extension of a Python program?
- Does the computer care what you type in as input? That is, will it accept complete nonsense just the same as your actual name?
- Define the word 'concatenate' in your own words.

## Errors

Introduce some errors to your program. After each error, save and try to run your program again. What error message is given for each of the following mistakes:

- Spelling one of the `print` statements with a capital P.
- Try spelling the `name` variable as `Name` in the input statement but do not change it in the print statement.
- Indent one of the statements in the program.

## You try...

Extend the program by prompting the user to tell where they were from and then print a reply. Output for that block of code might look like this:

    Where were you born, Jon?
    >>> Chicago
    That's interesting. I'd like to visit Chicago one day.

Have the program ask a several more questions to simulate a conversation.
