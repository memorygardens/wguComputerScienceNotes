You have already learned that a Cascading Style Sheets (CSS) document is an external text file that determines how to display the look and feel of HTML elements in your Webpages. It contains formatting instructions that can define the font, color and phrase elements used on a particular markup page.

If all pages on your site are linked to the same external style sheet, then one simple change to the style sheet will change all elements across the site. If you then want to change those instructions (for example, the style of <h1> headings), you need not change every page manually. You need only change a line in the style sheet file, then all your <h1> headings will change their appearance to conform to the style sheet. This technology can save a great deal of development and maintenance time, as well as make a more consistent, accessible interface.

## Benefits of Using CSS

CSS was created to solve a problem with HTML. The developers of HTML intended the standard to identify only the content and structure of a document, such as <title> and <body>, not the style, look and feel of the content.

When style elements for HTML4 were introduced without style sheets, the HTML standard grew complicated very quickly. Developers had to check each page of a Website to ensure it had the correct style tags for each element. Imagine the time and difficultly involved with this task.

To save developers from insanity, the W3C quickly went into action and standardized CSS. It greatly simplifies the application of style to Websites. Today a background image can be added to all Webpages with one change to an external CSS file.

CSS benefits include:

-   **Consistency** — CSS easily gives an entire site a consistent look and feel.
-   **Easy change management** — You can change the look and feel of an entire site by simply changing one part of a single line of code, rather than having to change possibly thousands of lines in hundreds of Webpages.

### CSS Syntax

Syntax:

selector {

      property: value;

}

Example:

      body {

            background-color: #000000;

            border: solid 1px #000000;

      }

In the above example, the:

-   selector is body
-   properties are background-color and border
-   values are #000000 and solid 1px #000000
-   This style rule contains two declarations

o   background-color: #000000;

o   border: solid 1px #000000;

-   style rule begins with the body selector and ends with the closing curly brace }

Selector: any element, class, or ID you want to style.

When styling a class, use a period ( . ) followed by the class value. Example: .special

When styling an ID, use a hash ( # ) followed by the ID value. Example: #wrapper

Visit W3Schools to learn more about [CSS Syntax](https://www.w3schools.com/css/css_syntax.asp).

### CSS Inheritance

The concept of inheritance is essential to CSS. In fact, the word "cascading" refers to inheritance. The style you define will flow, or cascade, throughout the documents, unless another style defined inside of a page specifically overrides it. Many styles can be used

together to create a completely formatted document. For example, a style sheet rule will override the default <body> font color, which is black. All these characteristics, whether they are defined in a style sheet or exist by default, are inherited throughout the rest of the document.

One important exception to the inheritance rule is the !Important directive. This directive allows you to overwrite the normal cascading that happens in a CSS style sheet. For example, imagine that you have a style sheet that reads:

p { color: blue; }

p { color: red; }

p { color: green; }

In this example the paragraph text would be displayed as green because that is the final style property that is applied. To make the text color red you could apply the !Important directive. It would read:

p { color: blue; }

p { color: red !important; }

p { color: green; }

To make the text color blue you would input:

p { color: blue !important; }

p { color: red; }

p { color: green; }

The !important declaration is one that you should use sparingly. It can work for a quick fix, but if it is overused it can negatively impact the way the CSS is processed. Over reliance on the !important declaration can also cause you to develop lazy programming tendencies. Developer consoles can be used in Web browsers to view and edit CSS on the fly. The functionality and focus of the tools provided depends on the Web browser you are using. The Chrome DevTools for the Google Chrome browser offer many different functionalities

and the ability to view the source code of any Webpage. You can easily access the Chrome DevTools by right clicking a Webpage and clicking the Inspect button. The Chrome DevTools allow you to view and make changes to CSS, HTML5 and JavaScript. You can learn more about the Chrome DevTools at _https://developers.google.com/web/tools/chrome-devtools/_.

Visit W3Schools to learn and practice more with CSS [Specificity](https://www.w3schools.com/css/css_specificity.asp) and ![important](https://www.w3schools.com/css/css_important.asp).

### Three Ways to Apply CSS

There are three ways in which you can apply CSS to a webpage. They are as follows:

·        inline (considered a bad practice)

·        internal style sheet

·        external style sheet (considered the BEST practice)

Visit W3Schools to learn and practice with the different [ways to apply CSS](https://www.w3schools.com/css/css_howto.asp) to HTML.

### Inline CSS Example

<p **style****="color:red;"**>This is a paragraph.</p>

### Internal CSS Example

<!DOCTYPE html>  
<html>  
<head>  
**<****style****>**  
**body {  
  background-color: linen;  
}  
  
h1 {  
  color: maroon;  
  margin-left: 40px;  
}  
</style>**  
</head>  
<body>  
  
<h1>This is a heading</h1>  
<p>This is a paragraph.</p>  
  
</body>  
</html>

### External CSS Example (Best Practice)

HTML File:

<!DOCTYPE html>  
<html>  
<head>  
**<****link** **rel****="stylesheet"** **href****="styles.css"****>**  
</head>  
<body>  
  
<h1>This is a heading</h1>  
<p>This is a paragraph.</p>  
  
</body>  
</html>

CSS File: styles.css:

body {  
  background-color: #ccc;  
}  
  
h1 {  
  color: #000066;  
  margin: 5px;  
}

### CSS Comments

Comments are helpful notes within a CSS file that provide more information about the purpose of style rules. The syntax for a CSS comment is:

/* Place comments here */  
 

### Syntactically Awesome Style Sheets (SASS)

Syntactically Awesome Style Sheets (SASS) is a CSS extension language that can act as a preprocessor to CSS. SASS, like other CSS preprocessors, enables you to add various special features to normal CSS, such as variables and nested rules. SASS is used in conjunction with CSS to make CSS code simpler and run more efficiently. CSS preprocessors offer valuable shortcuts and functionality, but it is not recommended to use a CSS preprocessor until you have mastered the core concepts of CSS.

Visit W3Schools to learn more about [SASS](https://www.w3schools.com/sass/default.php).

## Images

Images are commonly used within webpages. The <img> tag is used to place an image on a webpage. See example below:

<img src=”logo.png” alt=”Company logo”>

The <img> tag is an empty or void tag, meaning that it does not include a closing tag.

The required attributes for the <img> tag include:

-   src: short for source. The src attribute value is the name of the image file.
-   alt: short for alternative text. The alt attribute is makes the image accessible.

### Image File Formats

The following are the three image file formats used within a webpage:

-   Joint Photographic Experts Group (JPEG)
-   Graphics Interchange Format (GIF)
-   Portable Network Graphic (PNG)

**_JPEG_**

The Joint Photographic Experts Group (JPEG) format supports up to 24 bits of color information (16.7 million colors), and is typically used for photographs and complex images. It has small file size. In comparison to a similar sized PNG image, a JPEG image can have a much smaller file size.

This format also supports compression, meaning that you can reduce the image's file size. However, the more an image is compressed, the more its quality is reduced. For this reason, standard JPEG image compression is called "lossy" compression. JPEG compression is copyrighted in many countries. As a result, applications that use JPEG and other copyrighted materials may cost more or have limitations placed on them.

JPEG is supported in all major, modern browsers.

**_GIF_**

Graphics Interchange Format (GIF) files support 256 colors, rather than the millions of colors available to JPEG images. GIFs are best suited for line art, custom drawings and navigational images.

GIF has two versions:

-   GIF 87a
-   GIF 89a

GIF 89a is more popular because it supports the following techniques:

-   **Transparency** — the ability to make any part of the image invisible so the page background shows through. The image thus appears to blend into the background.
-   **Interlacing** — the ability for an image to render gradually as it downloads.
-   **Animation** — a series of images appearing in sequence to create the effect of motion.

GIF is supported in all major, modern browsers.

**_PNG_**

Portable Network Graphics (PNG) has emerged as a standard format for images on the Web and is widely implemented. PNG bit depth can be adjusted, unlike GIF and JPEG, which must be 8-bit and 24-bit depth, respectively. PNGs also use compression filters that can support up to 48-bit color. The PNG format was developed using open standards, which means that it does not have the same legal liabilities as other formats (e.g., GIF).

PNG brings together the best features of the GIF and JPEG formats into one format. PNG images provide the following features:

-   **Transparency** — similar to GIF 89a.
-   **Interlacing** — similar to GIF 89a.
-   **Compression** — lossless, unlike standard JPEG compression. Also, the compression used in the PNG format is not copyrighted, which has helped ensure developer and user agent vendor support.
-   **Animation** — less popular than animated GIF, but still relevant. Has the file extension APNG.

PNG is supported in all major, modern browsers.

**Image File Formats and Features Comparison**

**File Format**

**Transparency**

**Interlacing**

**Compression**

**Animation**

GIF 89a

Yes

Yes

Yes

Yes

JPEG

No

No

Yes

No

PNG

Yes

Yes

Yes

Yes

[Information about GPG](https://www.redhat.com/sysadmin/encryption-decryption-gpg)

### CSS and Images

**Image Backgrounds**

You can use CSS to specify an image as a background. See example below.

body {  
  background-image: url("wood_planks.gif");  
}

Visit W3schools to learn and practice making a [background image](https://www.w3schools.com/css/css_background_image.asp).

**Image Alignment**

You can use the CSS float property to place images to the left or right of text. See the example below.

Let’s say that you have the following <img> tag:

<img src=”product.jpg” alt=”text that describes the product in the picture” class=”floatright”>

Using the class, we can style the image to appear on the right with the following style rule:

img.floatright {

float: right;

margin: 2px;

}

### Resizing Images

Every image has a specified height and width (image size or dimensions). It’s important to understand the implications of manually specify dimensions in HTML if different from the original dimensions.

For example, let’s say that you have an image that is 500px wide by 300px tall. If you wanted the image to appear smaller on your page, use CSS to adjust the width and/or height using percentages. For example:

img {

     width: 50%;

     height: 50%;

}

The above style rule will reduce the image’s size by 50%, but maintain its aspect ratio so that the image does not appear stretched or distorted.

Now let’s use another example. Let’s say that you have an image that is 300px wide by 300px tall. And let’s say that you want to the image to appear larger on the page, so you specify an HTML width attribute of 600px and an HTML height attribute of 600px. That’s double the original file size! What do you think that will do to the image? Will the image look right on the webpage? No! The image will appear “pixelated” because you’ve forced the image to appear double its original size. Avoid doing this.

How do I find out the dimensions of an image file? Simple. Navigate to the image file, select the image file, right-click the file, and then select Properties. The image file dimensions can be found on the “Details” tab (Windows).

## COLORs

When applying colors using CSS, you can use color names, hexadecimal, RGB, or HSL.

### Hexadecimal

Hexadecimal (hex) color is commonly used to specify colors for CSS. It uses the following format: #RRGGBB. The RR represents the red color value. The GG represents the green color value. The BB represents the blue color value.

Colors are often specified in terms of their RGB values. RGB stands for Red Green Blue. You may know that if you were mixing paint, the mixture of red, green and blue together creates a rather muddy color. But on a monitor screen, you are mixing light, and the mixture of red, green and blue light produces white, which is the presence of all colors. Black is the absence of all colors. In RGB code, the higher the numeric value representing a color, the lighter that color will be. The lower the value, the darker the color. 

Colors are specified in RGB values ranging from 0 to 255. The hexadecimal value FF represents 255. Therefore, the hexadecimal value #FFFFFF represents the highest possible value for all three RGB colors, producing white. The hexadecimal value #000000 represents the absence of all colors, or black.

When the hex color value is the same for all 6 characters, you can use the shorthand and shorten to 3. For example:

The hex for white is #FFFFFF and the shorthand is #FFF.

**_Colors to know:_**

-   Black is #000000 (or #000)
-   White is #FFFFFF (or #FFF)
-   Red is #FF0000
-   Green is #00FF00
-   Blue is #0000FF

Visit W3Schools to learn more about [hexadecimal colors](https://www.w3schools.com/css/css_colors_hex.asp).

### More Color Value Options

**RGB**

Visit W3Schools to learn about [rgb() values](https://www.w3schools.com/css/css_colors_rgb.asp).

**HSL**

Visit W3Schools to learn about [hsl() values](https://www.w3schools.com/css/css_colors_hsl.asp).

### CMYK

CMYK is an alternative color scheme that is not supported in HTML5. CMYK stands for Cyan, Magenta, Yellow, and Key. The key color in CMYK is black. When you combine the RGB colors you produce the white color, while when you combine the CMYK colors you produce the black color. CMYK is currently used for color printing, so when you print an RGB color scheme on a color printer it will convert the RGB color scheme to a CMYK color scheme. This can result in some minor discoloring between the original and the print. CMYK is expected to be supported for Web browsers in HTML6.

### Browser-Safe Color Palette

Today’s modern monitors support millions of colors. Older monitors did not have the same capability, so 20 years ago, it was necessary to use the “browser-safe” or “web-safe” color palette, which consists of 216 colors.  This is no longer a necessary precaution, as all modern-day monitors can display the full color palette.

For more information about the [web-safe color palette](https://www.w3schools.com/colors/colors_shades.asp), visit W3Schools (scroll down to “Web Safe Colors?”)

## Link States

By default, hyperlinks that have not been clicked or selected are blue and hyperlinks that have been clicked are purple. You can use CSS to change these default colors using a pseudo-class link state for an anchor element. A pseudo-class is used to define the state of an element. For example, whether or not an element has been clicked. There are four link states for anchor elements, which include:

/* unvisited link */  
a:link {  
  color: #FF0000;  
}  
  
/* visited link */  
a:visited {  
  color: #00FF00;  
}  
  
/* mouse over link */  
a:hover {  
  color: #FF00FF;  
}  
  
/* selected link */  
a:active {  
  color: #0000FF;  
}

For more information about [pseudo-classes](https://www.w3schools.com/css/css_pseudo_classes.asp), visit W3Schools.com.

## Fonts (Text)

CSS allows you to specify many properties related to fonts, including the color, font family, font size, and more.

-   **_font-family_** — specifies the typeface (i.e., font name) to be used. A _font-family_ value must include quotation marks if it has multiple words, such as "Times New Roman." **_You should also list [fallback fonts](https://www.w3schools.com/css/css_font_fallbacks.asp) in the font-family value, such as Times New Roman, Arial, and Verdana. If the first font is not supported, the next value will attempt to render_**.
-   **_font-size_** — takes values in pixels, with 16 being the normal size of default text. The _font-size_ value is specified with the "px" abbreviation for "pixels." No spaces can exist between the number value and the abbreviation. For example, _font-size=16 px_ would not render properly, but _font-size=16px_ (with no space) would work correctly. Headings (h1 through h6) should be used whenever possible instead of the _font-size_ property.
-   **_color_** — uses the same values that you learned for specifying a page background color.

For more information about [CSS text properties](https://www.w3schools.com/css/css_text.asp), visit W3Schools.com.

## Web Design Issues

When creating a website, there are several important design aspects to keep in mind to avoid issues with poor design.  
 

### Color Combinations

Use contrasting colors in your design and be careful to not use too many colors, as this could be distracting.

Color combinations are important to a Website's look and feel because they can impose tone and mood. Color choices can convey the personality of a site, and thus its sponsoring organization, as serious, playful, trendy, conservative, creative, studious or authoritative, for example. Certain color combinations can also make a site easier — or more difficult — to read and view.

The following are some examples of popular color combinations for Websites:

-   Once a color scheme is chosen, most sites use lighter shades of chosen colors for background.
-   A lighter background acts as a foil (i.e., contrast) to the foreground text and images, making the site appear more polished and professional.

Visit W3Schools to view and play with [color schemes](https://www.w3schools.com/colors/colors_monochromatic.asp).

### Page Layout

Webpage layout is the placement of all page elements — including text, images, headings, navigation menus and so forth — relative to each other. A good page layout makes the page aesthetically pleasing, and easy to scan, read and navigate. Following are some layout guidelines to consider when designing your Webpages:

-   **Be succinct** — Limit words to clear, necessary verbiage, especially on the home page. Most users simply scan pages quickly looking for specific information or links to it. Let users navigate to additional pages if they want more information.
-   **Make sure that each page focuses on one topic** — No tangent message, regardless of its importance, should be added to a page. Use links to point users to appropriate related topics on separate pages.
-   **Divide the page into three sections** — Use the left side of the page for navigation, the upper section of the page for a topic title (as well as navigation), and the middle section of the page for the information.
-   **Include navigation aids** — A common way to enable navigation is to place links at the top and bottom of the page, and within the body of the page, to reduce the need for users to scroll.
-   **Place comments in each section of code** — Comments help explain changes you have made to the code or page. You can indicate the nature of the change, including the date you made the change and your name or initials, or you can explain the nature of the markup. For example, the aboutus.html page has three headings (h1, h2 and h3). You could comment each of these sections of the narrative.

### Document Structure and Style Sheets

When Webpages were first being developed, early designers would use the <table> tag to format pages. Tables were necessary to divide the pages into sections because the Cascading Style Sheets (CSS) standard had not yet been developed. By using tables, designers could ensure that all page elements aligned and rendered consistently.

Today, the use of the <table> tag to format pages is considered improper practice by the W3C. Pages formatted with the <table> tag will not pass W3C validation tests, no matter what standard you use. Following the use of tables, developers began to add structure to an entire page by using the <div> tag. It provided a way of dividing a page using an _id_ attribute. Once a name was specified for a document section using the _id_ attribute, developers could define this section's place in the document (as well as its contents) in a linked style sheet. That strategy gave developers granular control over the document and ensured that the style sheet — rather than the HTML tags — governed the document's structure.

HTML5 with CSS has introduced a more effective and simple way to structure Webpages. Instead of using the <div> tag as a "jack of all trades" element with its array of attributes, the developers of HTML5 created specific elements to define the document structure. These elements include <header>, <footer>, <nav>, <article>, and <aside>.

The following is an example of a basic HTML5 semantic wireframe:

<header>

<nav>

<article>

<article>

<article>

<footer>

The following are common HTML5 Semantic elements:

-   **<header>** — Top of the Webpage, similar to the header in a word-processing document.
-   **<nav>** — Defines navigation links, such as hypertext menus to access various pages of the Website.
-   **<main>** — Defines the main content area of a webpage.
-   **<article>** — Website content, such as company services, articles, blogs, images and videos.
-   **<aside>** — Content that is "aside" from the article content, such as advertisements or news feeds.
-   **<footer>** — Bottom of the Webpage, similar to the footer in a word-processing document.

For more about [HTML5 Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp) or [Website Layout](https://www.w3schools.com/css/css_website_layout.asp), visit W3Schools.com.

### Layouts: Fixed vs. Liquid

Web designers have no control over their site visitors' browser window sizes, the Web browsers used or the fonts installed on visitors' computers. Yet despite this, many designers try to control the way that Webpage elements will render on the screen. There are two page-layout methods that designers use to control the placement of Webpage elements when rendered in the browser:

-   **Fixed-width layout** — also known as absolute positioning. Achieved by assigning specific pixel widths to elements using the HTML5 structural elements or the <div> tag. This layout ensures that the text, images and layout will not vary from browser to browser. The problem with using a fixed-width layout is that the elements may not render as expected when users change the size of their browser windows.
-   **Liquid layout** — also known as relative positioning. Achieved by assigning percentage values to elements. With this layout, the size of an element is flexible and will change dynamically depending on the size of the browser window. For example, you can specify in the CSS width property that Element A will occupy 35 percent of the screen and Element B will occupy the remaining 65 percent. If the user resizes the browser window, the elements will resize correspondingly.

### Relative Path Names

Most Web developers use subfolders to organize images, style sheets and Webpages. Currently, your HTML pages are configured to refer to all images and style sheets in the same directory (e.g., a folder on your Desktop). As the site grows, your HTML pages will refer to subdirectories. A reference to a file within a directory or subdirectory is called a relative path.

A relative path statement allows you to specify subdirectories (i.e., subfolders), as well as directories above the one where your page currently resides. A relative path assumes that the directory in which the HTML file resides is the current (i.e., "home") directory. All other directories exist either beneath the current directory (i.e., subdirectories) or above the current directory (i.e., parent directories) in a hierarchical structure.

For example, if you place the uCorpCollage2.png file into the aboutus\ directory, and your Webpage's <img> tag needs to reference this image file, then you must change your _src_ attribute value to include the new subdirectory location, as follows:

<img src="images/logo.png" alt="company logo">

If you omit the subdirectory reference to images/ before the image file name, then your HTML page will look for the logo.png image file in its existing directory, and not in a subdirectory named images. Thus, the page will render without the image file, and a small box with an X will appear in its place.

### White Space and the <img> tag

With HTML, if you add a space or use the ENTER key to create a return within the <img> tag, the additional space will not be rendered in a browser. In XHTML, however, sometimes adding spaces or hard returns within or even between <img> tags will cause white space to appear on the page. Therefore, be careful when working with <img> tags in XHTML so that you do not add unintentional white space.

### Legacy Browers

HTML5 is not supported by Internet Explorer 8 or earlier. This is a challenge because the legacy operating systems cannot run Windows XP and Vista cannot run IE9 or above, which are the only Internet Explorer versions that supports HTML5. The simple solution is to install the latest version of the Chrome or Firefox browsers on Windows XP and Vista systems.

But what about your site visitors? You cannot force them to install Chrome or Firefox. They may be using IE8, 7 or 6. The only way to support these older IE browsers is to add JavaScript code to your HTML documents and a new rule to CSS. Because older IE browsers will not recognize the new HTML5 elements, such as <header>, <footer>, <article>, etc. JavaScript must be used to create these elements in your Webpage so older IE browsers will recognize them.

Note: JavaScript coding is beyond the scope of this course. This code is provided to demonstrate how JavaScript is used to support older browsers.