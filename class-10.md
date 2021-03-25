# Eror Handling & Debugging

When you are writing JavaScript, do not expect to write it perfectly the first time. Programming is like problem solving: you are given a puzzle and not only do you have to solve it, but you also need to create the instructions that allow the computer to solve it. too. 

The JavaScript interpreter uses the concept of __execution contexts__. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope. 

Every statement in a script lives in one of three execution contexts: 

* GLOBAL CONTEXT
Code that is in the script, but not in a function. There is only one global context in any page.

* FUNCTION CONTEXT 
Code that is being run within a function. Each function has its own function context. 

* EVAL CONTEXT 
Text is executed like code in an internal function called eval().

The first two execution contexts correspond with the notion of scope (Global scope & Function-level scope).

The JavaScript interpreter processes one line of code at a time. when a statement needs data from another function, it **stacks** (or piles) the new function on top of the current task.
If a JavaScript statement generates an error, then it throws an __exception__. At that point, the interpreter stops and looks for exception-handl ing code. 

Error objects can help you find where your mistakes are. When an Error object is created, it will contain the following properties: 

| Property | Description |
|-----|-----|
| name | Type of execution |
| message | Description |
| fileNumber | Name of the JavaScript file |
| lineNumber | Line number of error |

There are seven types of built-in error objects in JavaScript. 
* Error
* Syntax Error
* ReferenceError
* TypeError 
* RangeError
* URIError
* EvalError

The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.

You can pause the execution of a script on any line using __breakpoints__. Then you can check the values stored in variables at that point in time. 

If you set multiple breakpoints, you can step through them one-by-one to see where values change and a problem might occur. 

You can indicate that a breakpoint should be triggered only if a condition that you specify is met. The condition can use existing variables. 

You can create a breakpoint in your code using just the __debugger__ keyword. When the developer tools are open, this will automatically create a breakpoint. You can also place the debugger keyword within a conditional statement so that it only triggers the breakpoint if the condition is met.

```
var $form, width, height, area; 
$form = $('#calculator') ; 
$('#calculator').on('submit',function(e){
    e.preventDefault(); 
    consol e.log('Clicked submit...'); 
    width = $('#width').val(); 
    height = $('#height').val() ; 
    area = (width*height); 
    if (area < 100) { 
        debugger;      // A breakpoint is set i f the devel oper tools are open 
    $form.append('<p> ' + area + '</p>'); 
}) ; 
```

## Handling Exceptions

If you know your code might fail, use __try__, __catch__, and __finally__. Each one is given its own code block.
``` 
try { 
    // Try to execute this code 
} catch (exception) { 
    // If there is an exception, run this code 
} finally { 
    // This always gets executed
} 
```

If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.

`throw new Error( 'message');`

