# Lists

There are three types of HTML lists: ordered, unordered, and definition.

## Ordered lists

The ordered list is created with the **ol** element.

Each item in the list is placed within **li** element. (The li stands for list item.)

## Unordered lists

The unordered list is created with the **ul** element.
Each item in the list is also placed within **li** element. 

## Definition lists

The definition list is created with the **dl** element and usually consists of a series of terms and their definitions. Inside the **dl** element you will usually see pairs of **dt** and **dd** elements.

**dt** is used to contain the term being defined (the definition term). while **dd** is used to contain the definition.


# Boxes

CSS treats each HTML element as if it lives in its own box. You can set several properties that affect the appearance of these boxes.

## Box dimensions

By default a box is sized just big enough to hold its contents. To 
set your own dimensions for a box you can use the _height_ and _width_ properties.

Some page designs expand and shrink to fit the size of the user's screen. In such designs, the _min-width_ property specifies the smallest size a box can be displayed at when the browser window is narrow, and the _max-width_ property indicates the maximum width a box can stretch to when the browser window is wide. In the same way that you might want to limit the width of a box on a page, you may also want to limit the height of it. This is achieved using the _min-height_ and _max-height_ properties.

Every box has three available properties that can be adjusted to control its appearance:

1. Border

 The border separates the edge of one box from another, and has many properties:

- border-width
- border-style
- border-color
- border

2. Margin

Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes, and has many properties:

- margin-top
- margin-right
- margin-bottom
- margin-left

3. Padding

Padding is the space between the border of a box and any content contained within it, and has many properties:

- padding-top
- padding-right
- padding-bottom
- padding-left

The padding and margin properties are very helpful in adding space between various items on the page.

The **display** property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page. The values this property can take:

- inline
This causes a block-level element to act like an inline element.

- block

This causes an inline element to act like a block-level element.

- inline-block

This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.

- none
This hides an element from the page.

The **visibility** property allows you to hide boxes from users but It leaves a space where the element would have been.

The **border-image** property applies an image to the border of any box. It takes a background image and slices it into nine pieces.

# Arrays

An array is a special type of variable. It doesn't just store one value; it stores a list of values.

You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array). 

`var colors= ['white', 'black', 'custom'];`

Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one). Each item in an array is automatically given a number called an **index**. This can be used to access specific items in the array. 

Each array has a property called **length**, which holds the number of items in the array. 

` numColors =colors.length; `

# Decisions & Loops

## if ... else Statements

The **if ... else** statment checks a condition. if it resolves to **true** the first code block is executed. if the conidition resolves to **false** the second code block is run instead.

```
if (score >= 50){
    congratulate;
}
else{
    encourage;
}
```

## Switch Statements

A **switch** statement starts with a variable called the **switch value**. Each case indicates a possible value for this variable and the code that should run if the variable matches that value. 

```
switch (level) { 
    case 'One ': 
        title= 'Level 1 ' ; 
        break; 
    case 'Two': 
        tit 1 e = ' Level 2 ' ; 
        break; 
    case ' Three' : 
        title = 'Level 3' ; 
        break ; 
    default : 
        title= 'Test'; 
        break; 
}
```

## Loops

Loops check a condition. If it returns **true**, a code block will run. Then the condition will be checked again and if it still returns **true**, the code block will run again. It repeats until the condition returns **false**. There are three common types of loops:

1. For

```
For (var i=0; i < 10; i++){
    document.write(i);
}
```

2. While

```
while (i < 10) { 
    msg += i + ' x 5 = ' + (i * 5) + '<br I>'; 
    i++; 
}
```
3. Do While

```
do { 
msg += i + ' x 5 = ' + (i * 5) + '<br I>' ;s 
i++; 
} wh il e ( i < 1) ; 
```

