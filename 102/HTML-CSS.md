# Process & Design

Every website should be designed for the target audience—not just for yourself or the site owner. Therefore, it is very important to know exactly your audiences needs, and they are looking for. So, first thing we will discuss a process to use when we are creating a new website.

## Who is the Site For?

First of all, you have to answer the question about the people you would expect to be interested in the subject of your site, as it might be helpful to ask some to answer that question for you. The following question can help you answer the question you are looking for.

### Target Audience: individuals 
- What is the age range of your target audience?
- Will your site appeal to more women or men? What is the mix?

### Target Audience: Companies
- What is the size of the company or relevant department?
- Will visitors be using the site for themselves or for someone else?
- What is the position of people in the company who visit your site?

Now pick some fictional visitors from target audience.

| Name | Yousef | Fakhri | Salem |
|-----|-----|-----|-----|
| Age | 23 | 26 | 27 |
| Location | Amman | Zarqa' | Aqaba |
| Occupation | Engineer | Dentist | Programmer|

## Why People Visit YOUR Website

Now that you know who your visitors are and what are their backgrounds, we need to answer **why** they are coming. As the majority of the people will visit your website for a specific reason.

- Are they looking for general
entertainment or do they
need to achieve a specific
goal?
- If there is a specific goal, is
it a personal or professional
one?
- Do they see spending time on
this activity as essential or a
luxury?

## What Your Visitors are Trying to Achieve

It is unlikely that you will be able to list every reason why someone visits your site but you are looking for key tasks and motivations. This information can help guide your site designs.

**Ahmad** had a bad experience staying in a hotel when visiting Aqaba, Jordan, and wants to make a complaint.

**Amal** hopes to study architecture and wants to learn more about a new course that is being offered.

**Sami** is a picture editor and wants to look at a photographer's site to see examples of his work before deciding whether to commission him.

## What Information Your Visitors Need

You know who is coming to your site and why they are coming, so now you need to work out what information they need in order to achieve their goals quickly and effectively.
You may want to offer additional supporting information that you think they might find helpful.
By ensuring that you provide the information that your visitors are looking for, they will consider your site more relevant to them.

## Key Information

- Will visitors be familiar with your subject area / brand or do you need to introduce yourself?
- Will they be familiar with the product / service / information you are covering or do they need background information on it?
- What are the most important features of what you are offering?
- What is special about what you offer that differentiates you from other sites that offer something similar?
- Once people have achieved the goal that sent them to your site, are there common questions people ask about this subject area?

# HTML5 Layout

HTML5 introduces a new set of elements that allow you to divide up the parts of a page. The names of these elements indicate the kind of content you will find in them. They are still subject to change, but that has not stopped many web page authors using them already.
For example, the header sits inside a new **<header>** element, the navigation in a **<nav>** element, and the articles are in individual **<article>** elements.

## Headers & Footers

The **<header>** and **<footer>** elements can be used for:
- The main header or footer that appears at the top or bottom of every page on the
site.
- A header or footer for an individual **<article>** or **<section>** within the page.

## Navigation

The <nav> element is used to contain the major navigational blocks on the site such as the primary site navigation.

## Articles
The <article> element acts as a container for any section of a page that could stand alone and potentially be syndicated.
If a page contains several articles (or even summaries of several articles), then each individual article would live inside its own **<article>** element.

## Asides
The **<aside>** element has two purposes, depending on whether it is inside an **<article>** element or not.

When the **<aside>** element is used inside an **<article>** element, it should contain information that is related to the article but not essential to its overall meaning. For example, a pullquote or glossary might be considered as an aside to the article it relates to.
When the **<aside>** element is used outside of an **<article>** element, it acts as a container for content that is related to the entire page. For example, it might contain links to other sections of the site, a list of recent posts, a search box, or recent tweets by the author.

## Sections

The **<section>** element groups related content together, and typically each section would have its own heading.

Because the **<section>** element groups related items together,
it may contain several distinct **<article>** elements that have a common theme or purpose.

The **<section>** element should not be used as a wrapper for
the entire page (unless the page only contains one distinct piece of content). If you want a containing element for the entire page, that job is still best left to the **<div>** element.


## Heading Groups
The purpose of the **<hgroup>** element is to group together a set of one or more **<h1>** through **<h6>** elements so that they are treated as one single heading.


## Figures 

It can be used to contain any content that is referenced from the main flow of an article (not just images).

Examples of usage include:
- Images
- Videos
- Graphs 
- Diagrams 
- Code samples
- Text that supports the main body of an article

The **<figure>** element should also contain a **<figcaption>**
element which provides a text decription for the content of the **<figure>** element. In this example, you can see a **<figure>** has been added inside the **<article>** element.

## Sectioning Elements

The **<div>** element is an important way to group together related elements, because you should not be using the previous  elements that was mentioned for purposes other than those explicitly stated. 

Where there is no suitable element to group a set of elements, the **<div>** element will still be used.

## Helping Older Browsers Understand

Older browsers that do not know the new HTML5 elements will automatically treat them as inline elements. Therefore, to help older browsers, you should include the line of CSS below which states which new elements should be rendered as block-level elements.
```
<!--[if lt IE 9]>
    <script src="http://html5shiv.googlecode.com/svn/
         trunk/html5.js"></script>
<![endif]-->
```

# The Evolution of HTML

Since the web was first created, there have been several different versions of HTML. Each new version was designed to be an improvement on the last (with new elements and attributes added and older code removed).

There have also been several versions of each browser used to view web pages, each of which implements new code. Not all web users, however, have the latest browsers installed on their computers, which means that not everyone will be able to view all of the latest features and markup.

Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using (although browsers usually display the page even if it is not included). We will therefore be including one in each example for the rest of the book.

**HTML 5** 
`<!DOCTYPE html>`
**HTML 4**
```
<!DOCTYPE html PUBLIC
"-//W3C//DTD HTML 4.01 Transitional//EN"
"http://www.w3.org/TR/html4/loose.dtd">
```
**XHTML 1.0**
```
<!DOCTYPE html PUBLIC
"-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/
 xhtml1-strict.dtd">
 ```

## Comments in HTML

If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters:

`<!-- comment goes here -->`

It is a good idea to add comments to your code because, no matter how familiar you are with the page at the time of writing it, when you come back to it later (or if someone else needs to look at the code), comments will make it much easier to understand.
Although comments are not visible to users in the main browser window, they can be viewed by anyone who looks at the source code behind the page.

## ID Attribute

Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore (not a number or any other character).

It is important that no two elements on the same page have the same value for their id attributes (otherwise the value is no longer unique).

```
<p id="pullquote">
    Every time I view the sea I feel a calming sense of security, as if visiting my ancestral home; I embark on a voyage of seeing.
</p>
```
The id attribute is known as a global attribute because it can be used on any element.

## Class Attribute

Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within a document, you will want a way to identify several elements as being different from the other elements on the page. For example, you might have some paragraphs of text that contain information that is more important than others and want to distinguish these elements, or you might want to differentiate between links that point to other pages on your own site and links that point to external sites. 
To do this you can use the class attribute. Its value should describe the class it belongs to. In the example below, key paragraphs have a class attribute whose value is important.
```
<p class="important">For a one-year period from November 2010, the Marugame Genichiro-Inokuma Museum of Contemporary Art (MIMOCA) will host a cycle of four Hiroshi Sugimoto exhibitions.</p>
 ```

## Block Elements

Some elements will always appear to start on a new line in the browser window. These are known as **block level** elements.
Examples of block elements are <h1>, <p>, <ul>, and <li>.
```
<h1>Hiroshi Sugimoto</h1>
<p>The dates for the ORIGIN OF ART exhibition are as follows:</p>
<ul>
<li>Science: 21 Nov - 20 Feb 2010/11</li>
<li>Architecture: 6 Mar - 15 May 2011</li>
<li>History: 29 May - 21 Aug 2011</li>
<li>Religion: 28 Aug - 6 Nov 2011</li>
</ul>
```
## Inline Elements

Some elements will always appear to continue on the same line as their neighbouring elements. These are known as **inline** elements.
Examples of inline elements are < a>, < b>, < em>, and < img>.
```
Timed to a single revolution of the planet around the sun at
a 23.4 degrees tilt that plays out the rhythm of the seasons,
this <em>Origins of Art</em> cycle is organized around four
themes: <b>science, architecture, history</b> and <b>religion</b>.
```

## Grouping Text & Elements In a Block

The <div> element allows you to group a set of elements together in one block-level box. For example, you might create a <div> element to contain all of the elements for the header of your site (the logo and the navigation), or you might create a <div> element to contain comments from visitors.
In a browser, the contents of the <div> element will start on a new line, but other than this it will make no difference to the presentation of the page. 
```
<div id="header">
<img src="images/logo.gif" alt="Anish Kapoor" />
<ul>
 <li><a href="index.html">Home</a></li>
 <li><a href="biography.html">Biography</a></li>
 <li><a href="works.html">Works</a></li>
 <li><a href="contact.html">Contact</a></li>
</ul>
</div><!-- end of header -->
```
## Grouping Text & Elements Inline

The <span> element acts like an inline equivalent of the <div> element. It is used to either:

1. Contain a section of text where there is no other suitable element to differentiate it from its surrounding text.
2. Contain a number of inline elements.

```
<p>
Anish Kapoor won the Turner Prize in 1991 and exhibited at the <span class="gallery">Tate Modern</span> gallery in London in 2003.
</p>
```

## Inframes

An **iframe** is like a little window that has been cut into your page — and in that window you can see another page. The term iframe is an abbreviation of inline frame.
One common use of iframes (that you may have seen on various websites) is to embed a Google Map into a page. The content of the iframe can be any html page (either located on the same server or anywhere else on the web).
An iframe is created using the <iframe> element. There are a few attributes that you will need to know to use it:
- **src**
The src attribute specifies the URL of the page to show in the frame.
- **height**
The height attribute specifies the height of the iframe in pixels.
- **width**
The width attribute specifies the width of the iframe in pixels.


```
<iframe
    width="450"
    height="350"
    src="http://maps.google.co.uk/maps?q=moma+new+york&amp;output=embed">
</iframe>
```
