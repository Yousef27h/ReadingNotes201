CSS allows you to create rules that specify how the content of  an element should appear. For example, you can specify that  the background of the page is cream, all paragraphs should appear in gray using the Arial typeface, or that all level one headings should be in a blue, italic, Times typeface.

# Color

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
