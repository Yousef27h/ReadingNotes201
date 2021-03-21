# Objects

Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names. 

If a function is part of an object, it is called a **method**.If a variable is part of an object, it is called a **property**.

![object](/img/Capture.JPG)

You can access the properties or methods of an object using dot notation. You can also access properties using square brackets.

![method](/img/Capture1.JPG)
![property](/img/Capture2.JPG)



# Document Object Model

The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window. 

The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. It is implemented by all major browser makers, and covers two primary areas: 

* MAKING A MODEL OF THE HTM L PAGE
* ACCESSING AND CHANGING THE HTML PAGE 

As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes. 

1. THE DOCUMENT NODE 
2. ELEMENT NODES 
3. ATTRIBUTE NODES 
4. TEXT NODES 


Accessing and updating the DOM tree involves two steps: 

1. Locate the node that represents the element you want to work with. 
2. Use its text content, child elements, and attributes. 

Methods that find elements in the DOM tree are called DOm queries.
When you need to work with an element more than once, you should use a variable to store the result of this query.
DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes. 

Methods that return a single element node:

1. getElementByld('id')
2. querySelector('css selector') 
3. getElementsByClassName('class')
4. getElementsByTagName('tagName')
5. querySelectorAll('css selector') 

