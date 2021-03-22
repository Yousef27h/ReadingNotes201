# CSS Layout

CSS treats each HTML element as if it is in its own box. This box will either be a **block-level** box or an **inline** box.

* Block-level elements: **h1, p, ul, li.**

* Inline elements: **img, b, i.**

If one block-level element sits inside another block-level element then the outer box is known as the **containing** or **parent** element.

## CSS has positioning schemes that allow you to control the layout of a page:

1. Normal Flow

This is the default behavior,  Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.


2. Relative Positioning

This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. 
```
p.example {
    position: relative;
    top: 10px;
    left: 100px;}
```
3. Absolute Positioning

This positions the element in relation to its containing element. Absolutely positioned elements move as users scroll up and down the page.

```
h1 {
    position: absolute;
    top: 0px;
    left: 500px;
    width: 250px;}
```


The **float** property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.
Anything else that sits inside the containing element will flow around the element that is floated.

When you use the float property, you should also use the **width** property to indicate how wide the floated element should be. If you do not, results can be inconsistent but the box is likely to take up the full width of the containing element (just like it would in normal flow).

The **clear** property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box.

## Creating Multi-Column Layouts

The following three CSS properties are used to position the columns next to each other:

* width

This sets the width of the columns.

* float

This positions the columns next to each other

* margin

This creates a gap between the columns.

```
.column1of2 {
    float: left;
    width: 620px;
    margin: 10px;}
.column2of2 {
    float: left;
    width: 300px;
    margin: 10px;}
```

```
.column1of3, .column2of3, .column3of3 {
    width: 300px;
    float: left;
    margin: 10px;}
```

## Fixed width layouts

Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.

## Liquid layouts

Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.


There are two ways to add multiple style sheets to a page:

1. Your HTML page can link to one style sheet and that stylesheet can use the **@importrule** to import other style sheets.

`@import url("tables.css");`

2. In the HTML you can use a separate **link** element for each style sheet.

```
<link rel="stylesheet" type="text/css" href="css/site.css" />
<link rel="stylesheet" type="text/css" href="css/tables.css" />
 ```