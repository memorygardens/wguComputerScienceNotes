In creating a web site, you use standard HTML elements and tags to create functional documents.  These documents are commonly referred to as pages when written for the Web or for any other application.  The default or starting page of a Website is frequently called the home page for that site.

## Building a Web Site

When you create a web document, you can use any text editor and view it in any Web browser.

## Elements and Markup Tags

HTML elements are specific components of an HTML document that can provide content and attributes to a Webpage. Each element provides meaning to the page, such as identifying the title of the document or specifying where a video or audio file should be placed. These elements are interpreted by Web browsers and other user agents so that the Webpage renders properly.

In a nutshell, HTML documents can be described as a collection of elements. Without elements, a Webpage would have no structure or formatting.

Most HTML elements include a start tag and end tag, also called markup tags. Markup tags enclose elements in angle brackets, or wickets. Please note that the terms "elements" and "tags" are used interchangeably by many Web developers.

Tags embed the element information in the document so that a user agent will render text or other content as instructed by the associated element. For example, the **element is rendered using a start tag, <_strong_>, and an end tag, </_strong_>. The text surrounded by the start and end tag is rendered as bold font when viewed in a browser.**

**For example, bold text identified in an HTML document is written as:**

**_<strong>_****The text between the start and end tag of the strong element appears in bold when viewed in a web browser._</strong>_**

**The Web browser renders the HTML document text in bold, but the element and its tags do not appear:**

**Text between the start and end tag of the strong element appears in bold when viewed in a Web browser.**

**Use CSS when formatting or styling a Webpage and its elements.**

**For example:**

**Use font-weight in CSS instead of the <strong> tag when bolding text.**  

The combination of elements, markup tags and standard text is loosely referred to as either code or markup. Although markup languages are not programming languages, the elements and tags instruct the browser to perform certain actions, and so the use of the term "code" is appropriate in this context.

### Container tags and empty tags

There are two types of HTML tags:

-   **Container tags** — tags that come in pairs. Container tags use starting and ending tags. For example, when you want emphasis (italic) text, you will contain the text between starting and ending tags. These tags are also called the opening and closing tags. Container tags are also known as non-empty tags. Examples of container tags include:
    -   <html> ... </html>
    -   <head> ... </head>
    -   <body> ... </body>
    -   <p> ... </p>
    -   <div> ... </div>
    -   <header> ... </header>
    -   <footer> ... </footer>

-   **Empty tags** — tags that stand alone. Empty tags are those that do not directly format a specified block of text, and therefore one tag can execute the instruction. For example, if you want to create a line break, you insert the <br> tag at the point you want the break to occur. Empty tags are also referred to as void tags, standalone tags, or self-closing tags. Examples of empty tags include:
    -   <br>
    -   <hr>
    -   <meta>
    -   <link>
    -   <img>
    -   <source>
    -   <input>

### What constitutes a tag?

A tag can consist of the following three items inside the angle brackets:

-   **An element** — provides the main instruction of the tag. An element is required in every tag. Elements include <body>, <p>, <h1>, <title>, <table> and many others.
-   **An attribute** — specifies a quality or describes a certain aspect of the element. For example, a hyperlink is added to a Webpage by using the <a>, or anchor, element. The _href_ attribute is added, which identifies the hyperlink reference. Many elements require specified attributes, but some do not. An attribute is required in a tag only if the element requires it
-   **A value** — gives value to the element and its attribute. For example, <a href="http://www.w3schools.com"> has a value that instructs the hyperlink to access the W3Schools Website. Like attributes, values are optional in a tag unless required by a specified attribute to the element. Values are used only with attributes; elements do not take values directly. Values should be surrounded by quotation marks.

## Document Structure Tags

HTML5 documents usually contain most of the following document structure components:

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image001.png)**<!DOCTYPE> declaration** — The <!DOCTYPE declaration is the first tag in an HTML document. It informs the interpreter (usually a Web browser) what version of HTML the Webpage is written in. Previous to HTML5, the <!DOCTYPE> declaration was an SGML statement and required a fairly complex declaration. In HTML5, however, the tag is written as only <!DOCTYPE html>. The declaration is not case-sensitive, but it is almost always written in uppercase letters by Web developers (it will be uppercase in this course).

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image001.png)**<html>** **tag** — The <html> tag is used as a container for the entire HTML document. It nests all code except for the <!DOCTYPE> declaration.

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)**<head> tag** — The head section allows you to insert <meta> tags (which describe the nature of the document), links to style sheets, and the <title> tag

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image003.png)**<meta> tags** — The <meta> tag can specify various information about the document, known as metadata. This metadata can include a document description, revision dates, and keywords to help search engines index the page. It also specifies the HTML5 character set used, which is usually UTF-8. The <meta> tag is placed within the <head> container tags.

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image004.png)**<link> tag** — The <link> tag references a style sheet and is recommended for HTML5. A style sheet usually has a .css file name extension and a file name similar to the page to which it is linked (e.g., aboutus.css for the HTML page named aboutus.html). Style sheets are often placed in a subdirectory for the Webpage. This subdirectory contains all images and associated files for the page. The <link> tag is placed within the <head> container tags.

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)**<title> tag** — This tag identifies the document title. Most browsers will display the title in the browse's title bar. The <title> tag is placed within the <head> container tags.

**<body>** **tag** — This tag begins the body of the document and includes all the content of the Webpage, such as the text, video, hyperlinks, and images. The <body> tag is placed after the <head> tag.![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image003.png)

If your document fails to include these basic structure elements, it may still validate, given the flexible nature of HTML5. However, the document may or may not render in older browsers that do not support HTML5, such as Internet Explorer versions prior to IE9. You will learn more about backward-compatibility issues later in this course.

These basic structural elements are greatly simplified from previous HTML and XHTML versions. The following code displays the basic HTML5 document structure tags:

<!DOCTYPE html>

<html>

<head>

<title>HTML5 Structural Elements</title>

<meta charset="utf-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<meta name="author" content="Jose Santiago">

<link rel="stylesheet" type="text/css" href="stylesheet.css">

</head>

 <body>

<p>As you learn HTML5, you will start with the structural elements common to most HTML documents.</p>

</body>

</html>

Previous HTML and XHTML documents were different because the <!DOCTYPE> declaration included a Document Type Definition (DTD) file which referenced a specific HTML or XHTML standard. The DTD file is no longer required in HTML5. For example:

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" http://www.w3.org/TR/xhtml1/DTD/xhtml1- transitional.dtd>

### Are HTML tags case-sensitive?

HTML tags are not case-sensitive, but older XHTML tags are case-sensitive. Because XML is case-sensitive in that it requires strict conformance to letter case specified in a given DTD, it was decided that all XHTML document elements and attributes should be developed in lowercase letters to ensure consistency, compatibility and conformance.

The benefit to writing code in lowercase is that the code is now compliant with both HTML and XHTML and will render in all user agents that follow W3C standards. This practice has been widely adopted for all HTML coding.

### Document type declaration (<!DOCTYPE>)

The **document type declaration**, or <!DOCTYPE> declaration, describes the markup language and version of your code. It is placed at the very top of your document.

Prior to HTML5, the <!DOCTYPE> declaration was technically not XHTML or HTML; it was SGML. It included a reference to the Document Type Definition (DTD) for the markup version used. For instance, the [XHTML 1.0 Transitional <!DOCTYPE> declaration contained a reference to _www.w3.org/TR/xhtml1/DTD/xhtml1_](http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd)_-_ [_transitional.dtd_.](http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd)

Be careful not to confuse the document type declaration (<!DOCTYPE> declaration) with the Document Type Definition (DTD). The <!DOCTYPE> declaration is a statement that identifies code versions in a document.

The DTD is a separate, older document containing a set of rules for structure, syntax and vocabulary, used commonly with XHTML and XML. Previous versions of HTML also included a <!DOCTYPE> declaration that contained a DTD document reference. The DTD applied the rules of the specified language version.

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image005.png)If you do not specify a <!DOCTYPE> declaration, then two problems may arise: You may not be able to control how your code renders in the future.

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image006.png)You will not be able to use a markup validator, because the validator cannot determine the type of markup you are using (e.g., HTML5, XHTML Transitional or HTML 4.01).

Some examples of <!DOCTYPE> declaration statements follow.

#### HTML 2.0

The following <!DOCTYPE> declaration is used for HTML 2.0 files:

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 2.0//EN">

#### HTML 3.2

The following <!DOCTYPE> declaration is used for HTML 3.2 files:

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 3.2 Final//EN">

#### HTML 4.01

The following <!DOCTYPE> declarations are used for files written in the specified flavors of HTML 4.01 (the Web addresses are optional):

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image007.png)**HTML** **4.01** **Transitional**

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "[http://www.w3.org/TR/html4/loose.dtd](http://www.w3.org/TR/html4/loose.dtd)">

#### ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)HTML 4.01 Strict

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "[http://www.w3.org/TR/html4/strict.dtd](http://www.w3.org/TR/html4/strict.dtd)">

#### ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image008.png)HTML 4.01 Frameset

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" "[http://www.w3.org/TR/html4/frameset.dtd](http://www.w3.org/TR/html4/frameset.dtd)">

### XHTML 1.0

XHTML 1.0 approximates the HTML 4.01 <!DOCTYPE> declarations. If you are using the XHTML Transitional flavor and you are not including XML in your document, there will be little difference between an HTML 4.01 and an XHTML 1.0 document. The following <!DOCTYPE> declarations are used for the specified flavors of XHTML 1.0 (the Web addresses are optional).

#### ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image009.png)XHTML Transitional

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "[http://www.w3.org/TR/xhtml1/DTD/xhtml1-](http://www.w3.org/TR/xhtml1/DTD/xhtml1-) transitional.dtd">

#### XHTML Strict

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "[http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd](http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd)">

#### ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image005.png)

#### XHTML Frameset

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" "[http://www.w3.org/TR/xhtml1/DTD/xhtml1-](http://www.w3.org/TR/xhtml1/DTD/xhtml1-) frameset.dtd">

### HTML5

HTML5 is not based on SGML, so the traditional <!DOCTYPE> declaration is not required and there is no DTD required. However, it is important to include the <!DOCTYPE> declaration to ensure the browser can identify the version of HTML used in the Webpage. The following <!DOCTYPE> declaration is used for HTML5 files:

<!DOCTYPE html>

By using the declaration, you will improve your page's ability to work with various browsers. The declaration

### The <html> tag

The opening and closing tags must encompass all markup for the entire page. The tag can include several attributes, including:

-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image011.png)**manifest** — an attribute used for offline browsing. It lists the address of the HTML document's cache manifest. The manifest attribute requires each page you want cached to include the attribute. This technique is considered more reliable than a traditional browser cache.
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image012.png)**lang** — configures the page to use a particular language. For instance, a Web document written in English would use <html lang="en"> and a document written in French would use <html lang="fr">. This attribute is helpful for search engines and speech synthesizers. It is a universal attribute that can be used with many different elements besides <html>.
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image011.png)**xmlns** — If your content needs to conform to XHTML, then specify the XML namespace attribute The default entry is _xmlns="_[_http://www.w3.org/1999/xhtm_](http://www.w3.org/1999/xhtml)_l"_.

### The <head> tag

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image004.png)The <head> and </head> tags encompass several page elements, including: The <meta> tag.

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image013.png)![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image003.png)The <link> tag that references a CSS3 file, if present. The <title> tag.

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image014.png)The <script> tag which is used to define a client-side script.

### The <meta> tag

The <meta> tag can specify various information, or metadata, about the document. Attributes of the <meta> tag include the following:

-   **charset** —specifies the **character set** used in HTML documents (which is often set by the Web server for HTML documents, rather than by the document itself). It usually specifies the **Unicode** character set, which is standard in today's Webpages:

<meta charset="utf-8">

-   **name** — values include "keywords," "description", "robot", "viewport" and "author. " This attribute must be accompanied by the _content_ attribute. The "keywords" value of the _name_ attribute allows you to specify individual words as the value in the accompanying _content_ attribute. The "description" value of the _name_ attribute allows you to specify entire sentences as the value in the accompanying _content_ attribute; these sentences display in search engines to describe the purpose of the document. The "robots" value of the _name_ attribute is used to instruct search engines whether or not to index your page and follow the links on your page. The "viewport" value of the _name_ attribute is used to define the user's visible area on the Webpage. This value allows you to control the dimensions and scaling of the page to optimally display a Webpage on different sized devices.
-   **http-equiv** — provides an HTTP header for the information of the content attribute. Is useful when you do not have access to your server's configuration. Values include "content-type", "default-style" and "refresh". The "content-type" value of the _http-equiv_ attribute specifies the type of character encoding in the document. The "default-style" value of the _http-equiv_ attribute specifies the preferred style sheet that will be used. The "refresh" value of the _http-equiv_ attribute specifies a time interval for the Webpage to refresh itself. The "refresh" value should be used sparingly, if at all.
-   **content** — When paired with the _name_ attribute, the _content_ attribute values can supply keywords, author name, page descriptions and so forth, as previously described. The _content_ attribute essential in search engine optimization purposes. Following are some examples.

To change the viewport for your Webpage, you can use the <meta> tag as follows:

<meta name="viewport" content="width=device-width, initial-scale=1.0">

If you want to use the <meta> tag to provide a detailed description of your page, use syntax similar to the following:

<meta name="description" content="You can enter a useful description of the page here. You can use sentences, as you would in an email or letter, but keep it concise.">

To specify the author of the Webpage, use the <meta> tag with the "author" value:

<meta name="author" content="Rosa Estelle Rodriguez">

An extended discussion of the <meta> tag is beyond the scope of this course. However, the <meta> tag is a very effective back-end tool for ensuring that your pages work well across networks. The <meta> tag was discussed in this section because it is placed within the document structure tags.

### The <link> tag

Style sheet references are specified with the <link> tag in the <head> section, usually before the <title> tag. The <link> tag and CSS3 are recommended for HTML5. The link must point to a CSS3 file that is simple ASCII text.

The syntax of the <link> tag is as follows:

<link rel="stylesheet" type="text/css" href="theme.css">

### The <title> tag

The <title> tag is the first tag that allows you to specify content that will appear on the page. Any text you enclose with this tag appears in the page title box at the top of a browser. This text also appears in the history list and on the page when printed. Title text becomes the Bookmark name if the page is bookmarked or added to a browser Favorites folder. The <title> tag is the most essential tag necessary to rank highly in search engine optimization.

### The <body> tag

All content viewed by a Web browser or other user agent needs to be placed between the <body> and </body> tags. This content includes text, images, video, tables, lists and hyperlinks. The <body> tag no longer has attributes with HTML5. The previous formatting attributes have been replaced by CSS3 and the inline CSS style attribute.

## Website File structure

When creating a Webpage, you must consider the site's structure. Your HTML and images will be uploaded to a server eventually, so it is always good practice to organize your files as you create them.

The HTML pages are usually placed in a directory, and all images and files used in that page are stored in subfolders with the same name.

Visit [File Paths at W3Schools.com](https://www.w3schools.com/html/html_filepaths.asp) for more examples.

## Preparing Your Development Environment

Before you begin creating Webpage code, you should:

-   **Obtain a text editor** — Most operating systems have their own editors, so you do not need to download and install one. However, you may prefer to obtain a text editor that automatically numbers lines so you can easily reference your code. It is best to use a text editor that automatically saves standard ASCII text. Applications such as Microsoft Word can save to standard ASCII text only if you explicitly command them to do so. Common text editors include Notepad, WordPad, Vi, Pico and Emacs.
-   **Install multiple browsers** — You will need to test your code in multiple environments.
-   **Set file preferences** — The Windows operating systems do not always show file name extensions by default. You will be working with files with various extensions (e.g., .html, .css3, .txt), so you will need to be able to see them. You can set preferences in Windows 10 by selecting Start and searching for "File Explorer Options", then selecting the View tab. Deselect the Hide Extensions For Known File Types check box so that you can view all file name extensions.

## Paragraph Formatting and Block-level Elements

Markup elements that affect an entire paragraph or multiple paragraphs are referred to as **block-level elements**. Elements that can affect something as small as a character or a word are referred to as **text-level elements**. Block-level elements are automatically preceded and followed by paragraph breaks. Text-level elements are not followed by breaks unless the breaks are manually added.

### Paragraph Breaks and Line Breaks

The most basic block-level element is the paragraph element. The line break element is technically a text- level element, but it is included here in the context of formatting paragraphs. The <p> tag defines the start of a new paragraph, and a closing </p> tag specifies the end of the paragraph.

The <br> tag inserts a simple line break into the document. Because the <br> tag usually breaks a line of text, it never spans words or multiple lines of text, as does the <p> tag.

The <br> tag does not use a separate closing tag, so it follows a unique tag syntax. A closing slash is appended to every line break tag to make it a stand-alone non-empty tag, as follows: <br/>

### Heading Levels

Even the most basic documents will usually include at least one heading, and more likely several. Denoting text as heading elements emphasizes the start of different sections on your page and draws attention to that text. Heading tags have built-in styles associated with them. For example, text formatted as a heading level 1 element is rendered by default in a large, bold, serif font.

HTML uses six heading styles. Heading tags are container tags that encompass the affected text. The <h1> and </h1> tags cause enclosed text to be rendered in the heading level 1 style; the <h4> and </h4> tags cause enclosed text to be rendered in the heading level 4 style, and so forth. The largest heading is level 1. Heading level 4 text is rendered the same size as normal text. Heading levels 5 and 6 are smaller than normal text and should be used sparingly, if at all. 

Because headings are block-level elements, they are automatically preceded and followed by paragraph breaks, regardless of the relative position of the element to other text in the source code. It is important to note that you cannot place any header elements within a set of tags. If you do, your code will not validate as HTML5 and it may not render properly.

### Tag Nesting Markup

You will often use multiple sets of tags to format some text. Placing a pair of tags within another pair of tags is called tag nesting. You must ensure that your code is properly nested. Proper nesting means that you must open and close a pair of tags within another pair. The following two examples show both proper and improper tag nesting techniques.

**Proper**: <h1> <em> ... </em> </h1>

**Improper**: <h1> <em> ... </h1> </em>

Notice that in the improper example, the <em> tag (for italic text) is opened within the <h1> tag, but then closed outside the </h1> tag. If you fail to properly nest code, your pages may still render in some user agents, but they will not validate and may fail to render in the future.

Similarly, heading tags (e.g., <h1>, <h2>) should not be used within formatting tags (e.g., <em>, <p>). This tag combination constitutes improper nesting because the elements are incompatible, and will therefore prevent your code from validating.

Another example of a nested element:

<div>

<p>This paragraph element is nesed within a div element.</p>

</div>

### Primitive Formatting with the <pre> tag

Sometimes, you may want to use text that has already been formatted in a table or with a **fixed-width font**, such as Courier or Lucida Sans Typewriter. With the preformatted text tag (<pre>), all line breaks and spacing will be displayed in the browser exactly as they appear in the original text. The <pre> tag does this by preserving line breaks, tabs, and multiple spaces where text in other tags do not do this. The text will display in a fixed-width font, usually Courier.

The <pre> tag allows you to display plaintext files in their original format. It is commonly used to display tabular data. The <pre> tag is a container tag, requiring a closing </pre> tag.

### Indenting and Centering Text

When you want to center a paragraph of text, you must use an inline CSS3 _style_ attribute in the paragraph tag. The syntax is as follows:

<p style="text-align:center"> This text is centered. </p>

In this example, the <p> tag encompasses the text you want to format. The _style_ attribute tells the browser that the paragraph text should be aligned to the specified value, "center".

You can use the _style_ attribute for many formatting functions. Most often, you will use it to format content in an individual HTML file when you are not using CSS3 or when you want to override the external CSS3 file. For example, you can center text, tables and images. You can also use the _style_ attribute to justify items to the right or left on a page. For example, consider the following code:

<p style="text-align:right"> This text is aligned to the right. </p>

In this example, the text would render on the right side of the page.

The <blockquote> tag indents a block of text. As its name suggests, it is often used to specify quotes within a Webpage. The <blockquote> tag has a cite attribute that specifies the source of the quote. Do not use <blockquote> tags within <p> tags, and do not use <h1> tags within <blockquote> tags. Doing so will prevent your code from validating.

### Additional Block-level Elements

You can incorporate additional block-level elements into your pages. These include forms, horizontal ruling lines, and lists.

By this point, you should understand how to use the most common block-level tags:

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image007.png)<p>

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image018.png)<h1> through <h6>

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image019.png)<div>

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image020.png)

## Inline/Text-Level Elements

Text-level elements can affect a section of text as small as a single character or as large as an entire page. In the discussion that follows, you will learn how to use several text-formatting elements to emphasize text and embellish your pages

### Bold and Italic Text

Simple text-level elements include the following:

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image021.png)<strong> for **bold** text

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image008.png)<em> for _italic_ text

Underlined text will not be covered in this course. As a general rule, you should never use underline because this convention designates hyperlinks in Webpage text. It will confuse your Webpage viewers. If you still want to use underlined text, visit the CSS page at [_www.w3schools.com_](http://www.w3schools.com/).

Text-formatting tags are simple to use. Open the tag before the text to be affected, and close the tag where you want that effect to end. Ensure that tags are nested properly: The tag that opens first closes last, and the tag that opens last closes first

### Phrase Elements and Font Style Elements

The <strong> element and the older <b> element both create bold text. However, each element accomplishes this effect differently. The difference is that <b> specifically means apply the bold font style, whereas <strong> indicates that the text is to be given a strong appearance. In short, <b> represents a font appearance instruction, whereas <strong> represents the weighting of the phrase relative to surrounding text. The <b> element is called a font style element; <strong> is called a phrase element. The same is true of the older <i> element and the current <em> element, respectively, which both create italic or emphasized text.

Outside of ancient rhetoric, there is no such thing as "bold" speech, but the term "strong" can be used both to denote bold text when printed and strongly spoken text when output through an audio device.

For printed output, you can use phrase and font elements interchangeably. However, if you are coding for the future (as you should be), you should consider how the markup might be used in a different context, then apply the most appropriate tag.

Many text-level phrase elements output the same appearance. For example, the <code>, <kbd> and <samp> tags all make text appear in a fixed-space font. Phrase tags distinguish normal italic text from word definitions or variable program code within the HTML document. Using phrase tags is also beneficial because it is much easier to search for a specific tag within an HTML file instead of searching all italic, fixed- space or bold text.

Below are the text-level phrase elements, their usage and their appearances.

**Phrase Element**

**Usage**

**Appearance**

**<em>**

For emphasis

_italic text_

**<strong>**

For stronger, bolder text

**bold text**

**<dfn>**

For word definitions

_italic_ text

**<code>**

For program code examples

fixed-space font

**<kbd>**

For user keyboard text to be typed

fixed-space font

**<samp>**

For program sample output

fixed-space font

**<var>**

For variable text in program code

_italic text_

## Lists

A common markup function is to create bulleted and numbered lists. Lists are compound, block-level elements. Encompassed within list definition tags are individual list item tags. A paragraph break automatically precedes and follows the entire list. Individual list items are separated automatically by single line breaks.

There are three types of lists:

-   **Ordered list** — a numbered list. Uses the <ol> element and requires a closing </ol> tag.
-   **Unordered list** — a bulleted list. Uses the <ul> element and also requires a closing </ul> tag.
-   **Description list** - a list of description terms and definitions. Uses the <dl> element and also requires a closing </dl> tag.

Both list types use identical syntax. Each list item is specified using the list item element:

**List item** — specifies list items in an ordered or unordered list. Uses the <li> element and requires a closing tag.

**Ordered List Example:**

<h2>Ordered List</h2>

<ol>

<li>This is the first numbered item.</li>

<li>This is the second numbered item.</li>

<li>This is the last numbered item.</li>

</ol>

**Unordered List Example:**

<h2>Unordered List</h2>

<ul>

<li>This is the first bulleted item.</li>

<li>This is the second bulleted item.</li>

<li>This is the last bulleted item.</li>

</ul>

**Description List Example:**

<dl>

  <dt>HTML</dt>  
  <dd>Stands for HyperText Markup Language</dd>  
  
  <dt>CSS</dt>  
  <dd>Stands for Cascading Style Sheets</dd>  
  
</dl>

## HTML Entities

HTML Entities are non-keyboard characters, such as the copyright symbol. To add these characters to a page, you use HTML Entities. HTML Entities begin with an ampersand ( & ) and end with a semicolon ( ; ). For example:

     &copy; will insert the copyright symbol ©

The following table includes examples of HTML Entities.

**Character**

**Entity Code**

Copyright ©

&copy;

Less than <

&lt;

Greater than >

&gt;

Registered trademark ®

&reg;

Visit W3Schools to view even more HTML [Entities](https://www.w3schools.com/html/html_entities.asp), [Symbols](https://www.w3schools.com/html/html_symbols.asp), and [Emojis](https://www.w3schools.com/charsets/ref_emoji.asp).

## Good Coding Practice

### Forward-Compatibility

Remember that good coding practice involves writing code for forward-compatibility. That means you should always make your code cleaner to allow an easier transition to updated standards in the future. Such practices include:

-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image001.png)Closing all tags.
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image007.png)Using lowercase letters within tags.
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image018.png)Surrounding attribute values with quotation marks.

###   Universal markup and consistency

As previously discussed, another facet of good coding practice is creating universal markup that applies W3C standards consistently and thus renders consistently across most or all browsers. Remember to choose one HTML standard for your Web document, pages or site, then apply that standard carefully and consistently throughout. Applying the syntax rules of multiple standards in the same document or site not only prevents your code from validating but also produces unexpected rendering results in your users' browsers.

Note that this point does not contradict the previous point about applying the stricter syntax rules of XHTML in your HTML documents for the purpose of forward-compatibility. Using stricter syntax than required will rarely produce output problems. Inconsistency is mostly an issue with the older HTML standards because their looser rules allowed some sloppier coding practices to render without penalty. Keep in mind that you should understand the requirements of whichever standard you are using, and be particularly aware of syntax and tag usage.

###   Readability

If you are coding an HTML page and you are the only one who will ever look at the code, you may think the appearance of your code does not matter. This statement is basically true. But suppose you must share your work with others. Some coding techniques provide better readability, and make finding and changing code a simple operation. Other coding techniques produce a busy, confusing format that makes it difficult to decipher and edit the code.

Both sets of code will render the same in a browser, but clearly one set of markup is easier to read than the other. Line breaks and indentations both make code much easier to read and understand. Suppose you were hiring someone to write HTML code for you. Would you be more inclined to hire the developer of the code on the left, or the developer of the code on the right? The code on the right is much more readable.

### Exceptions

In some cases, you may find it impossible to make the code more readable without affecting the way it renders in the browser. With older XHTML code involving images or the tag, you may find that entering random white space can affect rendering in certain browsers. Always try to make your code readable, but verify that it renders properly.

###   HTML Comments

You can add comments within your HTML source code which will not appear on the page. The syntax for including a comment within your HTML document is as follows:

_<!-- comment text here -->_

### When to use comments

When creating markup pages, you can use comments to:

-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image001.png)![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image009.png)"Comment out" code to see how a page will appear without a particular markup element. Inform others about important elements in the code you are creating.
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image032.png)![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image004.png)Remind yourself why you inserted a particular piece of code. Insert programming code, such as JavaScript.

### **Responsive Web Design**

Responsive web design implementation is the hallmark of a modern Webpage. When you build a Webpage using responsive design it will fit comfortably onto any reasonable screen size. It will look just as good on a small mobile phone as a large desktop monitor. Responsive design Webpages are built using fluid grids, flexible images, and media queries. These have the advantage over fixed width grids in displaying flexible and dynamic Webpages. In responsive design, all the elements on a Webpage will resize their widths in relation to one another as the screen size changes. Ethan Marcotte is credited with creating responsive web design and published [this article in "A List Apart"](https://alistapart.com/article/responsive-web-design/) in 2010.