# HTML Basics 
## Introduction 
The module will cover 
-	HTML basic elements
-	HTML structure and syntax
-	hyperlinks
-	lists 
-	tables
-	div and span tags 
-	elements, entities, and HTML5 tags

## Vocab

## HTML Basic Elements
1. ```<!DOCTYPE html>``` : the document type declaration is mandatory and informs the browser which version of HTML is being used. The value html indicates HTML version 5. A declaration is a statement that informs the browser of the information needed to correctly handle the elements within. In other words, the declaration tells the browser how to decode the tags that will follow. 
2. ``` <html>```: element that encompasses the whole document 
3. ```<head>```: the page header information
4.``` <title>```: informs the page title to be used by the browser to be displayed over the window or tab displaying the web page
5. ```<body>```: the page body that encompasses the text to be displayed by the browser
6.``` <h1> -> <h6>```: the headings of the web page main text that follow specific text formatting and text structure
7. ```<p>```: the paragraphs of the web page text that hold the regular text.
8. ```<br>```: the single tag to create a line break.
9. ```<hr>```: tag to display a change of context, usually displayed with a horizontal line.
10. ```<strong>```: a tag to modify the weight of text relative to surrounding text, which usually is equivalent to bold 

**Two types of HTML elements**
	One could easily divide HTML elements into two groups. The first group consists of elements that refer to parts of a document: headers, paragraphs, tables, forms, lists, and so on. ```<h1>, <p>, <table>, <ul>```We call this semantic HTML as they refer to the names of things; they describe what they are.  
	
   Another group contains the elements used to indicate how things look: how they are aligned, which font is used, if it is in bold or italics, and so on  ```<center>, <font>, <b>, <i>``` and we could call them presentational HTML. The same is true for HTML attributes.  class="green" or id="chapter" would be semantic, while width="150px" or valign="top" would be presentational.  

#### Tags for meaning. 
```<em>``` => emphasis on a word. 

```<strong> ```=> bolden a word. 

```<code>``` => allows you to add css into an html file. Built right into the html, inline 

```<pre> ``` => allows you to use the formating you have in html to display as you have it. Think of odd poems. 

### Lists
Another important organizational tool for web pages is the list, or enumeration, of contents. In HTML this is usually done with three different, but similar, structures:

	- The  <ul> element that represents unordered lists where bulleted items are the default (in the essential reading you can see how to use other symbols instead of bullets).
	- The <ol>element that represents ordered lists where Arabic numerals are the default (in the essential reading you can see how to use other symbols instead of Arabic numerals).
	- The  <dl> element that defines lists where the items are preceded by a defined HTML element. (Key Value Pair)

### Tables
As expected, HTML follows the same markup language philosophy to clearly set apart the data from its formatting. Therefore, the table data is informed using the ```<table>``` tag to encompass the table rows, each identified by the  ```<tr>```  tag.

   Each row element may contain either a table header, or a common row. If a row contains the table header, each cell (one per column) within the header row uses the ```<th>``` tag. However, if the row contains common (non-header) elements, the ```<td>``` tag is used to identify the contents of each cell.
	
	
### Span and Div tags
A web page is frequently composed of several sections that may have different styles. You have already seen some ways to define sections in HTML, using headings and paragraphs that follow some natural divisions linked to the content itself. In addition to headings, there are two HTML elements you can use to define sections that are exclusively linked to formatting purposes: 

1. The ```<div>``` tag defines a section that is intended to aggregate multiple lines into a block that follows a similar style.
2. The ```<span>``` tag defines an inline section of text that follows a similar style.
	
The ```<div>``` tag can be defined with the usual attributes for background, colors, and borders, and other formatting options can be used as the padding property, which defines the margins of the ```<div>``` block.

The ```<span>``` tag is often used to refer to portions of the text that will follow a specific style according to the intended semantics of the displayed content.

For example, the HTML portion provided defines a section using the ```<div>``` tag with a background color, a border, and a padding of 60 pixels. It also defines a ```<span>``` tag to highlight a portion of the text using a border.
	
### HTML5- specific tags 
- ```<header>``` This is used to contain the headline for a page or section. It typically contains a company logo and navigational elements.
- ```<footer>``` Footers typically contain links to other related information, contact info, and copyright statements. Make sure you keep the latter up-to-date. People will not trust the information on a site that has a date of two years ago.  
 - ```<nav>``` This container can be used for the main navigation portion of your site.  
  - ```<aside>``` This tag is very useful to place the component of your side that often is placed on the left, next to everything else.  
  - ```<article> and <section>``` These two are useful to better organize your document. You can use them for blog posts or, as the names suggest, articles or sections.  
 
### HTML Entities 
>  As we know, all tags begin with a < sign and end with a > sign. Just imagine you want to use one of those as part of your content. This just might confuse the browser. That is why we have HTML entities. HTML entities are strings that begin with an ampersand and end with a semicolon. This represents the ampersand itself: & A very useful HTML entity is the non-breaking space:   It allows you to insert one or more spaces in you content. To use the < or > sign in your content, we have: < and > Also very useful are &eur;, for the Euro symbol, © for the copyright sign, and ® for the Registered Trademark sign. Non-English characters can be represented as HTML entities as well, for example, é for é, è for è, and ê for ê. We recommend you look up some of the online references if you want to see a complete list.


