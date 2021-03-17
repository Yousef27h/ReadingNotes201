# Links

Links are created using the __a__ element. Users can click on anything between the opening __a__ element. You specify which page you want to link to using the href attribute.

`<a href="http://www.google.com">Google</a>`

types of links:

1. Absolute URL

When you link to a different website, the value of the hrefattribute will be the full web address for the site, which is known as an **absolute** URL.

`<a href="http://www.empireonline.com">`

2. Relative URL 

When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a **relative** URL.

`<a href="about-us.html">About</a></li>`

Every page and every image on a website has a __URL__ (or Uniform Resource Locator). The URL is made up of the domain name followed by the __path__ to that page or image.

To create a link that starts up the user's email program and addresses an email to a specified email address, you use the <a>element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to.

`<a href="mailto:jon@example.org">Email Jon</a>`

If you want a link to open in a new window, you can use the target attribute on the opening **a** element. The value of this attribute should be _blank.

`<a href="http://www.imdb.com" target="_blank">`


# Layouts

CSS treats each HTML element as if it is in its own box. This box will either be a __block-level__ box or an __inline__ box.

Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text.

Block-level elements: h1, p, ul, li
Inline elements: img, b, i

If one block-level element sits inside another block-level element then the outer box is known as the **containing** or **parent** element.

CSS has the following **positioning schemes** that allow you to control the layout of a page: 

* normal flow
* relative positioning
* absolute positioning

 Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.You specify the positioning scheme using the _position_ property in CSS. You can also float elements using the _float_ property.

Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.

__Resolution__ refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.