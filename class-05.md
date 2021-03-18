# Images

Images can be used to set the tone for a site in less time than it takes to read a description.

To add an image into the page you need to use an __img__ element. This is an empty element (which means there is no closing tag).

`<img src="images/sky.jpg" alt="An image for the sky" />`

It can carry the following attributes:

1. src

This tells the browser where it can find the image file.

2. alt

This provides a text description of the image which describes the image if you cannot see it.

3. title 

used to provied additional information about the image.

4. height
Specifies the height of the image in pixels.

5. width
 Specifies the width of the image in pixels.



# Color

CSS allows you to create rules that specify how the content of  an element should appear. For example, you can specify that  the background of the page is cream, all paragraphs should appear in gray using the Arial typeface, or that all level one headings should be in a blue, italic, Times typeface.

The color property allows you  to specify the color of text inside an element.Every color on a computer screen is created by mixing amounts of red, green, and blue. You can specify any color in CSS in one of three ways:

- ## RGB Values

These express colors in terms of how much red, green and blue are used to make it up.As they are expressed as numbers between 0 and 255, For example: rgb(100,100,90)


- ## HEX Codes

These are six-digit codes that represent the amount of red, green and blue in a color in hexadecimal code, preceded by a pound or hash **#** sign. For example: #ee3e80

- ## Color Names

There are 147 predefined color names that are recognized by browsers. For example: DarkCyan

CSS treats each HTML element as if it appears in a box, for example the **background-color** property sets the color of the background for that box.

# Saturation 

Saturation refers to the amount of gray in a color. At maximum saturation, there would be no gray in the color. At minimum saturation, the color would be 
mostly gray.

# Brightness

Brightness (or "value") refers to how much black is in a color.At maximum brightness, there would be no black in the color.At minimum brightness, the color would be very dark.

# Opacity

**opacity** is a property which allows you to specify the opacity of an element and any of its child elements.The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).

The CSS3 **rgba** property allows you to specify a color, just like you would with an RGB value, but adds a fourth value to indicate opacity.This value is known as an **alpha value** and is a number between 0.0 and 1.0(so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).

CSS3 introduces an entirely new and intuitive way to specify colors using **hue**,**saturation**, and **lightness** values.

**HUE**: Hue is the colloquial idea of color with a value from 0 to 360.
**SATURATION**: Saturation is the amount of gray in a color. Saturation is represented as a percentage. 100% is full saturation and 0% is a shade of gray.

**LIGHTNESS**: Lightness is the amount of white (lightness) or black (darkness) in a color. Lightness is represented as a percentage.0% lightness is black, 100% lightness is white, and 50% lightness is normal.

The **hsla** color property allows you to specify color properties using hue, saturation, and lightness as above, and adds a fourth value which represents transparency (just like the rgba property). The a stands for **Alpha** (This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency.)



# Text

The properties that allow you to control the appearance of text can be split into two groups:

- Those that directly affect the font and its appearance.
- Those that would have the same effect on text no matter what font you were using.

The font weight adds emphasis and can also affect the amount of white space and contrast on a page.

## SERIF

Serif fonts have extra details on the end of the main strokes of the letters.

## SANS-SERIF

Sans-serif fonts have straight ends to letters and therefore have a much cleaner design.

## MONOSPACE

Every letter in a monospace typeface is the same width. (Non-monospace fonts have different widths.)

## CURSIVE

Cursive fonts either have joining strokes or other cursive characteristics, such as handwriting styles.

## FANTASY

Fantasy fonts are usually decorative fonts and are often used for titles. They're not designed for long bodies of text.


The _font-family_ property allows you to control typeface for the text you want. 

The value of this property is the name of the typeface you want.

In  order for the people who are visiting your site to display it, they have to have that typeface on their computers.
You can have multiple typeface separated by comma, if the user does not have the first downloaded on his computer, the code will pick the second typeface.

The _font-size_ property enables you to specify the size of a font, using pixels (px), percentages (%), and ems (equivalent to the width of a letter m).

_@font-face_ allows you to use a font even if its not installed on the computer of the user browsing, as you specify a path to a copy of the font.

` @font-face {font-family: 'ChunkFiveRegular';src: url('fonts/chunkfive.eot');}`
