# Dictionary
## - 1 - What is CSS?
## - 2 - How To Add CSS?
## - 3 - CSS color Property
## - 4 - CSS reference
## - 5 - CSS Tools: Reset CSS
  ----------------
### What is CSS?
CSS (Cascading Style Sheets) allows you to create great-looking web pages, but how does it work under the hood? This article explains what CSS is, with a simple syntax example, and also covers some key terms about the language.

>Prerequisites:	Basic computer literacy, basic software installed, basic knowledge of working with files, and HTML basics (study Introduction to HTML.)
Objective:	To learn what CSS is.

In the Introduction to HTML module we covered what HTML is, and how it is used to mark up documents. These documents will be readable in a web browser. Headings will look larger than regular text, paragraphs break onto a new line and have space between them. Links are colored and underlined to distinguish them from the rest of the text. What you are seeing is the browser's default styles — very basic styles that the browser applies to HTML to make sure it will be basically readable even if no explicit styling is specified by the author of the page.

#### What is CSS for?
As we have mentioned before, CSS is a language for specifying how documents are presented to users — how they are styled, laid out, etc.

A document is usually a text file structured using a markup language — HTML is the most common markup language, but you may also come across other markup languages such as SVG or XML.

Presenting a document to a user means converting it into a form usable by your audience. Browsers, like Firefox, Chrome, or Edge , are designed to present documents visually, for example, on a computer screen, projector or printer.

Note: A browser is sometimes called a user agent, which basically means a computer program that represents a person inside a computer system. Browsers are the main type of user agent we think of when talking about CSS, however, it is not the only one. There are other user agents available — such as those which convert HTML and CSS documents into PDFs to be printed.

CSS can be used for very basic document text styling — for example changing the color and size of headings and links. It can be used to create layout — for example turning a single column of text into a layout with a main content area and a sidebar for related information. It can even be used for effects such as animation. Have a look at the links in this paragraph for specific examples.

#### CSS syntax
CSS is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page. For example "I want the main heading on my page to be shown as large red text."

The following code shows a very simple CSS rule that would achieve the styling described above:

>h1 {
    color: red;
    font-size: 5em;
}
The rule opens with a selector . This selects the HTML element that we are going to style. In this case we are styling level one headings (<h1>).

We then have a set of curly braces { }. Inside those will be one or more declarations, which take the form of property and value pairs. Each pair specifies a property of the element(s) we are selecting, then a value that we'd like to give the property.

Before the colon, we have the property, and after the colon, the value. CSS properties have different allowable values, depending on which property is being specified. In our example, we have the color property, which can take various color values. We also have the font-size property. This property can take various size units as a value.

A CSS stylesheet will contain many such rules, written one after the other.

>h1 {
    color: red;
    font-size: 5em;
}

>p {
    color: black;
}

You will find that you quickly learn some values, whereas others you will need to look up. The individual property pages on MDN give you a quick way to look up properties and their values when you forget, or want to know what else you can use as a value.

#### CSS Modules
As there are so many things that you could style using CSS, the language is broken down into modules. You'll see reference to these modules as you explore MDN and many of the documentation pages are organized around a particular module. For example, you could take a look at the MDN reference to the Backgrounds and Borders module to find out what its purpose is, and what different properties and other features it contains. You will also find links to the CSS Specification that defines the technology (see below).

At this stage you don't need to worry too much about how CSS is structured, however it can make it easier to find information if, for example, you are aware that a certain property is likely to be found among other similar things and are therefore probably in the same specification. 

For a specific example, let's go back to the Backgrounds and Borders module — you might think that it makes logical sense for the background-color and border-color properties to be defined in this module. And you'd be right.

### How To Add CSS
There are three ways of inserting a style sheet:

* External CSS
* Internal CSS
* Inline CSS

#### External CSS
With an external style sheet, you can change the look of an entire website by changing just one file!

Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.

Example
External styles are defined within the <link> element, inside the <head> section of an HTML page:

* <!DOCTYPE html>
* <html>
* <head>
* <link rel="stylesheet" href="mystyle.css">
* </head>
* <body>
* <h1>This is a heading</h1>
* <p>This is a paragraph.</p>
* </body>
* </html>

An external style sheet can be written in any text editor, and must be saved with a .css extension.

The external .css file should not contain any HTML tags.


#### Inline CSS
An inline style may be used to apply a unique style for a single element.

To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

Example
Inline styles are defined within the "style" attribute of the relevant element:

>> <!DOCTYPE html>
<html>
<body>
<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>
</body>
</html> 

## CSS color Property
### Definition and Usage
The color property specifies the color of text.

Tip: Use a background color combined with a text color that makes the text easy to read.
Set the text color with a HSL value:

body {color: hsl(89, 43%, 51%);}

## CSS reference
### Basic rule syntax

>Style rule syntax
> style-rule ::=
    selectors-list {
      properties-list
    }
... where :

> selectors-list ::=
    selector[:pseudo-class] [::pseudo-element]
    [, selectors-list]

> properties-list ::=
    [property : value] [; properties-list]

## CSS Tools: Reset CSS

The goal of a reset stylesheet is to reduce browser inconsistencies in things like default line heights, margins and font sizes of headings, and so on. The general reasoning behind this was discussed in a May 2007 post, if you're interested. Reset styles quite often appear in CSS frameworks, and the original "meyerweb reset" found its way into Blueprint, among others.

The reset styles given here are intentionally very generic. There isn't any default color or background set for the body element, for example. I don't particularly recommend that you just use this in its unaltered state in your own projects. It should be tweaked, edited, extended, and otherwise tuned to match your specific reset baseline. Fill in your preferred colors for the page, links, and so on.

In other words, this is a starting point, not a self-contained black box of no-touchiness.

If you want to use my reset styles, then feel free! It's all explicitly in the public domain (I have to formally say that or else people ask me about licensing). You can grab a copy of the file to use and tweak as fits you best. If you're more of the copy-and-paste type, or just want an in-page preview of what you'll be getting