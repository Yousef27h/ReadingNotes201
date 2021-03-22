# Tables

A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results.

## Basic Table Structure

The **table** element is used to create a table. The contents of the table are written out row by row.

You indicate the start and the end of each row using the **tr** element. (The tr stands for table row.) 

Each cell of a table is represented using a **td** element. (The td stands for table data.)

```
<table>
    <tr>
        <td>15</td>
        <td>15</td>
        <td>30</td>
    </tr>
    <tr>
        <td>45</td>
        <td>60</td>
        <td>45</td>
    </tr>
    <tr>
        <td>60</td>
        <td>90</td>
        <td>90</td>
    </tr>
</table
```
The **th** element is used just like the **td** element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.) 


# Constructor

We can create blank object using the **new** keyword and the the object constructor.

![constructor](/img/Coons.JPG)

To update the value of properties, use dot notation or square brackets.
To delete a property, use the **delete** keyword.

Sometimes you will want several objects to represent similar things. Object constructors can use a function as a template for creating objects. First, create the template with the object's properties and methods. 

The keyword __this__ is commonly used inside functions and objects. Where the function is declared alters what this means. It always refers to one object, usually the object in which the function operates.

Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages. 

1. BROWSER OBJECT MODEL 

The Browser Object Model contains objects that represent the current browser window or tab. It contains objects that model things like browser history and the device's screen. 

2. DOCUMENT OBJECT MODEL 

The Document Object Model uses objects to create a representation of the current page. It creates a new object for each element (and each individual section of text) within the page.

3. GLOBAL JAVASCRIPT OBJECTS 

The global JavaScript objects represent things that the JavaScript language needs to create a model of. For example, there is an object that deals only with dates and times. 
