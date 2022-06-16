When you want to display data that is best suited to a tabular format, you can use the set of table tags provided in HTML. Tables can provide useful and attractive grids for Webpage content.

Another option for displaying tabular data is the <pre> tag. It, however, is extremely limited in function. HTML tables allow images, alignment, color, and many customization attributes.

## The table Element

The <table> tag creates a table and contains all other table elements. The other HTML tags used to create a table are the <caption>, <tr>, <th>, and <td> tags.

### Syntax

<table>

<caption>This is table caption text</caption>

<tr>

<th>column header 1</th>

<th>column header 2</th>

</tr>

<tr>

<td>table cell 1</td>

<td>table cell 2</td>

</tr>

</table>

**Element**

**Tag**

**Required**?

**Description**

**Table**

<table> … </table>

Required

Creates a table. Contains all other table elements.

**Table Caption**

<caption> … </caption>

Optional

Adds a caption or title, which appears above the table by default.

**Table Row**

<tr> … </tr>

Required

Contains all data for a table row.

**Table Header**

<th> … </th>

Optional

Typically designates cells in the top row or left column. By default, text in a header cell will appear bold and centered.

**Table Data**

<td> … </td>

Required (unless <th> is being used)

Designates table cell contents. By default, the data is left-justified.

### CSS Properties for all table elements

### **Property**

### **description**

### **values**

### **border**

Determines the style of the border

-   Border width (e.g., 1px)
-   Border line style (e.g., solid)
-   Border color (e.g., gray)

### **border-collapse**

Collapses the borders of adjacent cells into a single border instead of separating them.

Collapse

### **border-spacing**

Determines the amount of space between the borders of adjacent cells.

Number of pixels

### **padding**

Determines the amount of space between cell data and the cell border.

Number of pixels

### **width**

Determines how far the table or cell will extend horizontally across the page.

-   Number of pixels
-   Percentage of the browser window – number followed by percent symbol (%)

### **background-color**

Determines the background color for table elements.

-   Color name (e.g., green)
-   Hexadecimal code (e.g., #00FF00)

### **text-align**

Aligns text horizontally

-   Left
-   Center
-   Right
-   Justify

### **vertical-align**

Aligns content vertically.

-   Top
-   Bottom
-   Middle

**Note**: Table data alignment can drastically affect the look of a table. For the best result, align content consistently within columns. The CSS3 property to specify horizontal alignment is text-align. For vertical alignment, use the vertical-align property.

Adding height and width to table header and data cells increased this table's readability. However, adding unnecessary height or width to your table can waste space on your Webpage.

The **_colspan_** and **_rowspan_** attributes can be used to force a cell to span multiple columns and/or rows.

As your tables become more complex, you will quickly understand why GUI HTML editors are so popular. It is still essential, however, that you create HTML tables manually, so you understand how to manipulate and customize tables created with GUI HTML editors.

HTML tables have often been used to create content structure for entire webpages. In HTML5, however, you should not use tables to structure a page. Instead, the W3C recommends that you use the new HTML5 document structure tags.

The HTML5 structure elements can be defined as:

-   **<header>** - Top of the Webpage, like the header in a work-processing document.
-   **<nav>** - Defines navigation links, such as hypertext menus to access various pages of the Website.
-   **<article>** - Website content, such as company services, articles, blogs, images, and videos.
-   **<aside>** - Content that is “aside” from the article content, such as advertisements or news feeds.
-   **<footer>** - Bottom of the Webpage, like the footer in a work-processing document.

Note: A search engine could automatically rank a page lower if the page uses tables for structure. Use tables tastefully and sparingly.

#### Bootstrap Tables

The bootstrap framework is an open-source, front-end framework that contains HTML and CSS design templates. It is widely used due to its mobile first outlook.

One useful table type that the Bootstrap framework provides is the responsive table.

You can learn more about Bootstrap responsive tables and the Bootstrap framework at [_https://www.w3schools.com/bootstrap/default.asp_](https://www.w3schools.com/bootstrap/default.asp).