# How HTML, CSS, & JavaScript Fit Together

- **HTML** (.html) This is where the content of the page lives. The HTML gives the page structure and adds semantics.
- **CSS** (.css) enhances the HTML page with rules that state how the HTML content is presented (backgrounds, borders, box dimensions, colors, fonts, etc.).
- **JavaScript** (.js) This is where we can change how the page behaves, adding interactivity. We will aim to keep as much of our JavaScript as possible in separate files. 

## How to use objects & methods

The **document** object represents the entire web page. All web browsers implement this object, and you can use it just by giving its name.

`document.write('Good afternoon!');`

The **write()** method of the **document** object allows new content to be written into the page where the **< script>** element sits.

## JavaScript runs where it is found in the HTML

when the browser comes across a **< script>** element, it stops load the script and then checks to see if it needs to do anything.

# Basic JavaScript Instructions

## Statements

A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a **statement**. Statements should end with a semicolon. 
The semicolon also tells the JavaScript interpreter when a step is over, indicating that it should move to the next step.

## Comments

You should write **comments** to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code. 

### MULTI-LINE COMMENTS 

To write a comment that stretches over more than one line, you use a **multi-line** comment, starting with the /* characters and ending with the */ characters. Anything between these characters is not processed· by the JavaScript interpreter. 

### SINGLE-LINE COMMENTS 

In a **single-line** comment, anything that follows the two forward slash characters I/ on that line will not be processed by the JavaScript interpreter. Singleline comments are often used for short descriptions of what the code is doing.


## Variables

A script will have to temporarily store the bits of information it needs to do its job. It can store this data in **variables**. 

Before you can use a variable, you need to announce that you want to use it. This involves creating the variable and giving it a name. programmers say that you **declare** the variable.


## Data Types

- Numeric Data Type : The numeric data type handles numbers.
- String Data Type: The strings data type consists of letters and other characters.
- Boolean Data Type : Boolean data types can have one of two values: true or false.


