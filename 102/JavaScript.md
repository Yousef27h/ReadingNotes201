# How JavaScript Makes Web Pages More Interactive

1. Access Content 
You can use JavaScript to select any element, attribute, or text from an HTML page. For example:
- Select the text elements that all of the **< h1>** elements on a page
- Select any elements that have a **class** attribute with a vles of **note**.
- Find out what was entered into a text input whose **id** attribute has a value of **email**.

2. Modify Content

You can use JavaScript to add elements, attributes, and text to the page, or remove them. For example:
- Add a paragraph of text after the first **< hl>** element
- Change the value of **class** attributes to trigger new CSS rules for those elements
- Change the size or position of an **< img>** element

3. Program Rules 
You can specify a set of steps for the browser to follow (like a recipe), which allows it to access or change the content of a page. For example:
- A gallery script could check which image a user clicked on and display a larger version of that image.
- A mortgage calculator could collect values from a form, perform a calculation, and display repayments.
- An animation could check the dimensions of the browser window and move an image to the bottom of the viewable area (also known as the viewport).


# The ABC of Programming

Before learning how to read and write the JavaScript language, we need to familiarize ourself with some key concepts in computer programming. 
as they will be covered in three sections:

- A : What is a script and how do I creat one?
- B : How do computers fit in with the world around them?
- C : How do I write a script for a web page?

## 1/a What is a script and how do I create one?

A **script** is a series of instructions that a computer follows to achieve a goal. for instance, we can compare scripts with recipes, handbooks, or manuals, since all of these books you have to follow set of rules in order to get to final result you want, same goes with scripts but the difference is the computer is the one who's following the instructions.
A **browser** may use different parts of the script depending on how the user interacts with the web page.


In order to write a script, you'll need first to state your goal and list the tasks that need to be completed in order to achieve it.

Humans tend to divide complex tasks into smaller and simpler tasks when they do it for the first time, with experience these individual tasks grow familiar and seem simpler.

Some of the scripts may seems complicated and might look intimidating at first. However, a script is just a series of short instructions, each of which is performed in order to solver the problem we have. 

**Start with the big picture of what you want to achieve, and break that down into smaller steps**. First define the goal, then design the script and this can be done using a **flowchart**. Finally, code each step in a programming language that the computer understands.

Each individual task may be broken down into a sequence of steps. When you are ready to code the script, these steps can then be translated into individual lines of code.

# Expressions

An **expression** evaluates into (results in) a single value. Broadly speaking there are two types of expressions.

1. EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE

`var color = 'beige';`

When you first declare a variable using the **var** keyword, it is given a special value of undefined. This will change when you assign a value to it.

2. EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE

You can perform operations on any number of individual values to determine a single value. For example:
`var area = 3 * 2;`


# Functions

Functions let you group a series of statements together to perform specific task. If different parts of a script repeat the same task, you can re-use the function (rather than repeating the same set of statements).

To create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces. This is known as a **function declaration**

Having declared the function, you can then execute all of the statements between its curly braces with just one line of code. This is known as **calling the function**. 

Some functions return information to the code that called them. For example, when they perform a calculation, they return the result.
