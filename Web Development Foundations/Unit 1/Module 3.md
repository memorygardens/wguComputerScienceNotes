# Cascading Style Sheets

## Vocabulary and Syntax
### Internal/Inline
> Inline is defined as inside the HTML file by using style tag. It will apply only to the portions that have side style inline in the tags, not the whole document

### External
> External is loaded after the HTML file and allows you to alter over multiple HTML files. This is the more common way to do a website or web project

### CSS Syntax
1. **Selector:** Are used to determine which html element the css is effecting. 
![[Pasted image 20220607232349.png]]
2**. Declaration Block:** is the portion that includes the Selector and the stylings on said Selector. 
![[Pasted image 20220607232451.png]]
3. **Declaration**: Are the styling rules in the Declaration Block. Set up in the Property Value split by : and ended with ;
4. **Comments** ```/* */ ```

**Guidelines for CSS :** [Code Guide](https://codeguide.co)

## Basic CSS Commands, aka Rule-Sets

**CSS Selector** 
>In CSS, selectors are patterns used to select the element(s) you want to style.
>[w3Schools](https://www.w3schools.com/cssref/css_selectors.asphttps://www.w3schools.com/cssref/css_selectors.asp)

**References** 
![[Pasted image 20220612175624.png]]

### Specificity
>If we have multiple CSS declarations that have equal specificity, the last declaration is the one that will be applied to the element.

The specificity of a CSS rule is a sequence of four numbers that are calculated as follows: 
1. If the rule is an inline style, the first number is 1, otherwise it is 0 
2. Add 1 to the second number for every occurrence of an identifier
3. Add 1 to the third number for every class specified
4. Increase the fourth number by one for every element present  
 
 
**Ranking**
1. universal (``*``)
2. type (p)
3. class (.example)
4.  id (#example) 

4 begin the override that trumps all the others 
![[Pasted image 20220612191114.png]]

Style declarations cascade and are read from top to bottom 
!important will take precedence no matter where it is placed  (not best practice)

### Block and Inline Elements 
CSS block elements are going to be rectangular areas of the document. These blocks can contain text, data, as well as other block elements. It should be noted that CSS block elements may only appear within a a body tag. Inline elements can only contain inline elements and cannot be given a width. Blocks can contain inline elements, not the other way round. 
Inline elements => anchor tags, span and strong. 
Block elements => paragraph, h1, article, section, div.

![[Pasted image 20220612200536.png]]

![[Pasted image 20220613195428.png]]

### Text Related Attributes 
Serif Fonts 
- Serif fonts are typefaces that have glyphs with small decorations or serifs at some of the edges of the letter. For example, the short lines at the bottom of each leg in the letter m.

Sans-serif fonts 
-	Sans-serif fonts are the counterpart of serif fonts. They do not contain the small decorations or serifs at the end of the stroke, hence the name sans (French for without) serif.  

Monospace Fonts 
- In the typefaces we have discussed so far, not all characters have the same width: the letter m is clearly wider than the letter i. A monospaced font, also called a fixed-width, is a font where letters and characters do indeed have the same width.  

-   `font-family`: defines the font type
    -   serif fonts are often used for paragraph text on a web page and include Times New Roman, Courier, Courier New, and Georgia
    -   sanserif fonts are often used for content headers and include Arial, Helvetica, and Geneva
-   `text-align`: defines the text alignment to be employed and the common values are left, center, right, and justify
-   `font-size`: defines how many pixels will be used for the current font, with the values expressed numerically by the following possible units:
    -   `px`(pixels): a tiny unit of illumination on a computer screen
    -   `em`: used to describe the proportion of the current font size (using the letter _m_); e.g. _2em_ indicates twice the size of the current font size
    -   `%`: used to describe the proportion of the current font of the body section, as compared to the size of the current font; e.g. 50% indicates that the font will be ½ the size of the body section.
    -   `vw`: used to indicate a proportion of the window size; e.g. _2vw_ corresponds to 2% of the number of pixels of the current viewport of the page (the window width)
-   `font-style`: defines the use of either normal, italic, or oblique font styles
-   `font-weight`: defines the use of normal or bold font-weight
-   `line-height`: defines the space occupied by each text line with common values being 1 for single space, 1.5 for one and a half-space, and 2 for double space, but in practice, any numerical value is accepted as a proportion of the standard line space
  
### Positioning
Float Property: float comes from the print world and allows you to move elements around 

### Styling 
Pseudo-class selectors => ':visted' is used to change the color of a link after it is clicked. 
We conclude our selection on CSS properties with the introduction of some pseudo-classes, typically but not solely used with , the anchor tag. The anchor tag is used mainly for links. To make it visible that they are indeed links, the default styling of happens to be a blue color and the text is underlined, which is not very attractive. Using pseudo-classes, you can give an anchor tag, in theory any tag, a different look depending on where the cursor is  
  
### Building a Web Page 
>  WYSIWYG (what you see is what you get) graphic editor

### Summary 
-   There are three ways to insert CSS instructions into HTML
    -   inline definition
    -   internal definition
    -   external definition
-   A rule-set contains the following:
    -   one selector
    -   set of declarations 
-   Specificity is a weight applied to CSS values to determine which CSS property value is applied.
-   When to use block and inline elements 
-   How color and text related attributes affect the web page 
-   How to use the box model for design and layout
-   How positioning and float can assist a developer with element layouts 
-   Styling methods
