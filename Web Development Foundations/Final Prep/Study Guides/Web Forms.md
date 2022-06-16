**Introduction to Web Forms**

Websites use forms to obtain input from users. You can create several types of fields in one form to collect various types of user input. Such input can include the user's name, address and credit card number, for example. The information a user enters into the form is then submitted to a server where it is stored and/or processed.

After a user has entered information into a Web form, he or she clicks the form's Submit button. Submitting the form uploads or emails the user's information to the receiving server. Many Web forms also provide a Reset button that clears entered data instead of submitting it, and resets the form fields to the default values.

Forms are of little use without an application on a Web server to process the submitted information. CGI scripts perform this information processing. The following sections discuss the ways that CGI scripts receive and process Web form information. The rest of the lesson will teach you how to develop Web forms using HTML.

**Web Forms and CGI**

To be truly functional, a Web form requires a combination of a Web server technology such as IIS, Tomcat or Apache Web Server and a **server-side scripting** processor such as PHP, ASP, or Java to interpret the form's input. In contrast, **client-side scripts** are executed on the client's computer or browser.

A Web server performs several important functions:

-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image003.png)Receives data from a Web form or a client-side script Processes and reformats input data
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image003.png)Stores data on server-side storage systems such as databases or file systems Resends data to other servers for further processing or storage
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image004.png)   Responds to client-side requests

Without server-side scripting languages, Web forms would not be able to communicate with clients. Web servers and server-side scripting languages are available for Linux/UNIX, Mac, and Windows operating systems and are relatively easy to install and maintain. These technologies are mostly available for free to use but require the purchase of a service agreement from company or a third party for sustained technical support. Some technologies do require a license to be used commercially so make sure to read the user agreement closely.

Another server-side technology that you may encounter is **Common Gateway Interface (CGI)**. CGI technologies pre-dates Web servers but are still used with software that is embedded in hardware as well as in many legacy applications that may still exist in the technical industry. CGI scripts act as an interface between client applications and servers and behave in a similar way as a Web server. They receive client input, process data, perform server-side actions such as storage or communications with other servers, and respond to client requests.

**Visualizing Client-Server Communication**

The following elements are necessary for client-server communication:

-   Web browser
-   Web form
-   Web server
-   Server-Side Scripting Language or a CGI script

A Web form processing script remains on a Web server. The Web forms you will learn to create in this lesson allow users to upload information to your Web server, where information can be processed and acted upon. Actions taken by the Web server and server- side script can include:

-   Storing information in a database (for example, bank account updates).
-   Searching a database for a product (for example, a book or movie at Amazon.com).
-   Sending processed information back to the end user (for example, a new bank account balance or a confirmation that a book was shipped).

You now understand that a CGI script residing on a server receives data from a Web browser, then processes the data into human-readable format (or any other format you require). Before a CGI script receives any data, however, a user must enter the data into a Web form and submit it.

A form allows the user to provide his name and email address, then indicate whether he wants to be placed on the company's mailing list. When the user clicks the Submit Query button, the browser sends the information entered in this form to the Web server as a raw text string.

The basic element of a raw text string is a name=value pair. The _name_ attribute of the

<form> element organizes information input by the user into name=value pairs. For example, the Web form in the preceding figure organizes user input according to the following code. Pay special attention to the code shown in bold:

Enter Your Name:

<input type="text" name="**Name**" size="40"> Enter Your Email: <input type="text" name="**Email**" size="40"> Should we add you to our mailing list? <br>

<input type="radio" name="**AddToList**" value="yes"> Yes

<input type="radio" name="**AddToList**" value="no">No

When the browser sends this data, it will use the _name_ attribute values "Name", "Email" and "AddToList" as the basis for creating the raw text string. You can specify any words as _name_ values. In this example, the server receives a raw text string that resembles the following:

Name=Dimitri+Pappas&Email=student50@class.com&AddToList=yes

This raw text string consists of name=value pairs, delimited by ampersands (&). In a name=value pair, entered spaces are replaced with plus signs (+). If a form field is left empty, only the first part of the name=value pair will be returned. For example, if this user left the mailing list option blank, the corresponding name=value pair would return "Email=" without any information after the equal symbol.

After the server receives this information, a CGI script can parse and format the raw text string into a human-readable format similar to the following:

**Name:**           Dimitri Pappas

**Email:**            [student50@class.com](mailto:student50@class.com)

**Mailing List:** Yes

The Web form you will create in this lesson will use Name and Email, as well as other name values that correspond to their functions. Now that you understand how a basic script processes Web form data, consider a commonly used CGI script: FormMail.

**Applied example: FormMail**

One example of a CGI script is the venerable FormMail script, written by Matt Wright. This script has existed in various versions since 1997. It is written in Practical Extraction and Report Language (Perl) and has the file name FormMail.pl. FormMail has not been maintained since 2009. Accordingly, it is outdated and poses security risks. It is still a useful tool for developing an understanding of Web forms, however, even if it would be inadvisable to use on a public facing Webpage.

FormMail is designed to receive information from a Web form via the Perl interpreter. The script then sends the form information to you via email. You simply check your email to receive results from the script. You can learn more about FormMail at Matt's Script Archive ([_www.scriptarchive.com/formmail.html_](http://www.scriptarchive.com/formmail.html)).

FormMail is popular for many reasons, including the following:

-   It is available free of charge from Matt's Script Archive (MSA).
-   It is written in Perl, which allows developers to use a free CGI interpreter available in many places, including [_www.cpan.org_](http://www.cpan.org/). Most modern operating systems allow the Perl interpreter to be installed, making Perl one of the more ubiquitous languages. The combination of a free, powerful Perl interpreter and a free, well-written FormMail script is widely appealing.
-   FormMail is easy to customize. Wright specifically designed FormMail for ease of use: The developer simply modifies a few portions of the script and it is ready to perform whatever tasks a particular Web form requires.

After you download FormMail, you perform the following simple steps:

-   Install Perl on your Web server. Many Web servers already have Perl installed.
-   Define the FormMail variables so that the script is capable of receiving information and sending it to you.
-   Give executable permissions to the FormMail.pl script on your Web server. 
-   Wait for users to visit your site, and then check your email for results.

Many organizations and businesses use the FormMail script for various beneficial purposes. Some companies have made money through Web-based sales. Other sites have used the script to help charities and other worthy causes.

##### **Security concerns**

Spam has become a concern for most Web users. Some unscrupulous individuals have taken advantage of the FormMail script because older versions could be fooled into sending email to anyone. Some systems administrators still use older versions of the program.

Other administrators improperly configure newer script versions, resulting in more spam on the Internet. You should use the latest version of FormMail, which has features that allow its use without inviting abuse from spammers.

##### **Other versions of FormMail**

You are not limited to using the original Perl FormMail script. Alternative versions of FormMail are available for PHP ([_https://www.tectite.com/formmailpage.php_](https://www.tectite.com/formmailpage.php)) and ASP ([_www.brainjar.com/asp/formmail_](http://www.brainjar.com/asp/formmail)), for example.

  
**HTML5 and Forms**

The basic form elements and attributes for form creation in HTML5 are little changed from HTML 4.01. The main differences are:

1.  Cascading Style Sheets (CSS3) are used for all form styles.
2.  Advanced features are now available, such as new <form> elements and attributes, and <input> types for better control of validation and input control.

At the time of this writing, many of the new elements and attributes are not supported by most browsers, even the ones that support HTML5. As HTML5 continues to evolve, these new elements and attributes will be adopted.

To learn more about the new HTML5 form elements and attributes, visit the W3Schools HTML5 Forms section at [_http://www.w3schools.com/html/_](http://www.w3schools.com/html/) and click the links in the HTML5 Forms navigation bar.

  
**Basic Tags for Creating Web Forms**

You can create a user-input Web form on a Webpage by placing HTML code to create various form fields in between a set of HTML <form> tags. Such forms are essential for receiving input from users and for e-commerce.

All elements of the form should be contained in the <form> element section in order for the form to function and process properly. There are many types of fields that you can place in a form, depending on the type of info you want to elicit from users. This section describes the basic HTML tags used to create a Web form. In the sections that follow, you will add a field type to your Web form with each successive lab.

  
**The <form> tag**

The HTML <form> tag creates a user-input Web form by encompassing all the content and fields of the form on the page. The <form> tag is a container tag, so you should include both opening and closing tags. In some older browsers, if you fail to supply the closing </form> tag, the form may not render or may not submit.

In HTML5, if you fail to supply the closing </form> tag, the form will still render and users can still submit data, because HTML5 is very forgiving of loose code (whereas earlier HTML and browser versions are not). However, omitting the closing </form> tag can still produce unexpected results in HTML5. For example, if you have two forms on your page and you omit the closing </form> tag at the end of the first form, data from the second form will be submitted with the first. Also, forms using JavaScript may not process as intended if you do not specify where your form ends. It is good coding practice to close your forms properly so you and other developers can more easily decipher your design intentions.

Syntax for a <form> tag:

<form method="post" action="example.php">

<input ...>

<select> ... </select>

</form>

For now, ignore the <input> and <select> elements.

The <form> element has two main attributes associated with it:

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image015.png)_method —_ specifies which method the browser will use to send form data to a Web server

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image016.png)_action —_ specifies the name and location of the CGI script used to process the form

These attributes are required in the <form> tag in order to process data that users submit in the form.

### **The method attribute**

The _method_ attribute specifies the method by which the browser will send form data to a Web server. The _method_ attribute takes two values:

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image017.png)"get" — Form data is appended to the URL of the Webpage for use in a query string. This method sends information in cleartext and is thus less secure.

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image018.png)"post" — Form data is posted to the URL specified by the _action_ attribute. Post is the preferred method for sending form data. It can send more characters, although sometimes post requires more processing by the CGI script.

### **Query strings**

All forms use form elements, such as an input element to enter your first name, last name, address, email, etc. Each input element (or select or textarea elements) include the name attribute assigned to some value. For example, an input element meant for a user to enter their first name might be: 

<input type=”text” name=”firstname” id=”firstname”> 

When the get method is used within a form, it appends the name-value pairs to the end of an URL as a query string. For example, let’s say your domain is exampledomain.com and the php file is named example.php. An example of a query string appended to the end of the URL would be: 

[http://www.exampledomain.com/example.php?firstname=John&lastname=Smith](http://www.exampledomain.com/example.php?firstname=John&lastname=Smith) 

The highlighted area above is the query string. It is appended at the end of the URL. The question mark (?) is used to append the query string.

### **The action attribute**

The _action_ attribute specifies the name and location of the CGI script used to process the form. The contents of the form will be processed by the script and acted upon according to the instructions in the script.

###   
**The <input>, <select> and <textarea> tags**

You can use the <input>, <select> and <textarea> tags to create form fields by placing them between the <form> </form> tags.

### **The <input> tag and the type attribute**

The <input> tag is not a container tag; it stands alone. You use <input> to create text boxes, check boxes, radio buttons, and the Submit and Reset buttons.

The <input> element takes the _type_ attribute. The value you use with the _type_ attribute designates the form field type as a text box, a radio button, a Submit or Reset button, a password field or a check box. For example, to create a radio button with the <input> element, you would use the following syntax:

<input type="radio" name="AddToList">

You can change the value of _type_ to create other buttons or fields. You can also add other attributes to customize the field's behavior. To create a password field, for example, you would use the following code:

Enter Your Password: <input type="password" name="Password" size="14">

### **The <select> tag**

The <select> tag is a container tag used to create single-option and multiple-option select lists. Following is an example of <select>:

How often do you want to be updated about uCorp?<br/>

<select name="frequency">

<option value="weekly">Once a week</option>

<option value="bi-weekly">Every other week</option>

<option value="monthly">Once a month</option>

<option value="none">Never</option>

</select>

When using the <select> tag, you may want to allow users to select more than one option from the list. If so, you must use the _multiple_ attribute with "multiple" as the value. For example, consider the following HTML code:

<p>Which countries have you worked in?</p>

<select name="Countries" **multiple="multiple"** size="4">

<option value="austrila">Australia</option>

<option value="newzealand">New Zealand</option>

<option value="england">England</option>

<option value="france">France</option>

<option value="india">India</option>

<option value="china">China</option>

</select>

This code allows users to select multiple countries, rather than just one.

### **The <textarea> tag**

The <textarea> tag is a container tag used to create an area for user commends and feedback. Following is an example of <textarea>:

<label for="comments">Comments:</label>  
  
<textarea id="comments" name="comments" rows="6" cols="20">  
Please add your comments here.  
</textarea>

The size of the <textarea> element is specified with the rows and cols attributes. [Visit W3Schools.com to practice.](https://www.w3schools.com/tags/tag_textarea.asp)

  
**Web Form Fields**

**Form Field**

**Description**

**Example**

**Text box**

A text field into which a user can enter characters.

[<input type="text">](https://www.w3schools.com/tags/att_input_type_text.asp)

**Radio** **button**

Round option buttons in a group of two or more mutually exclusive options.

[<input type="radio">](https://www.w3schools.com/tags/att_input_type_radio.asp)

**Check box**

Square boxes in a group of two or more non-exclusive options.

[<input type="checkbox">](https://www.w3schools.com/tags/att_input_type_checkbox.asp)

**Single- option** **select list**

A drop-down list of two or more options from which a single selection can be made.

[<select>](https://www.w3schools.com/tags/tag_select.asp)

**Multiple- option** **select list**

An exposed list of two or more options, optionally scrollable, from which the user can make multiple selections.

[<select multiple>](https://www.w3schools.com/tags/att_select_multiple.asp)

**Text area**

A scrolling text field into which the user can enter multiple lines of text.

[<textarea>](https://www.w3schools.com/tags/tag_textarea.asp)

**Password field**

A text box that visually masks the entered characters as filled circles.

[<input type="password">](https://www.w3schools.com/tags/att_input_type_password.asp)

**File upload**

A button and field that allow users to navigate to and select a local file for uploading or other purposes (for example, to validate HTML files).

[<input type="file">](https://www.w3schools.com/tags/att_input_type_file.asp)

**Submit** **button**

A button that, when clicked, causes the form's action statement to process.

Labeled "Submit" or "Submit Query" by default, but can display any label.

[<input type="submit">](https://www.w3schools.com/tags/att_input_type_submit.asp)

**Reset** **button**

A button that, when clicked, clears all form data and sets all form fields back to the default values for those fields.

Labeled "Reset" by default, but can display any label.

[<input type="reset">](https://www.w3schools.com/tags/att_input_type_reset.asp)

  
**Forms and the** **_name_** **attribute**

All form field elements share an attribute: _name_. The _name_ attribute identifies information you receive from a user and associates it with a value you specify. The _name_ attribute helps you organize user input. For example, you could use a series of check boxes to learn about a user's preferences for gardening, sailing and biking, and you could name the group of boxes "Interests." Thus when you receive information from the Web form, the names in your results clearly indicate the user's choices.

  
**Text boxes**

A text box is used to collect a single line of data from the user, such as name, email or address information. The text box is the most common form field.

The syntax for creating a text box is as follows:

<input type="text" name="FieldName">

If you want the text box to appear with some default text inside, use the additional _value_

attribute as shown:

<input type="text" name="FieldName" value="DefaultText">

Additionally, you can use a _size_ attribute to specify the width of the text box in characters. The _size_ attribute has no effect on the amount of text the user can enter; it restricts only the visual appearance of the field. Contrast this with the _maxlength_ attribute. The value of _maxlength_ restricts user entries to the specified number of characters; it has no effect on the display width of the field.

## **Identifying HTML form elements and attributes**

  
**File upload**

You can allow your site's users to upload files to your site using a Web form. Simply use the "file" value of the _type_ attribute to the <input> tag as follows:

Provide your resume here: <input type="file" name="UploadedFile">

This code will create a Browse button on the Web form. When a user clicks the Browse button, a Choose File dialog box will appear, which the user can use to navigate to and select a local file for uploading. An accompanying text box displays the path and file name that the user has chosen.

**Submit and Reset buttons**

When you specify the <input> tag's _type_ attribute value as "reset" or "submit", you create a button that performs a specific action. Clicking the Submit button sends the data from all fields in the form to be processed by the _action_ specified in the <form> tag. Clicking the Reset button clears all form fields instead of submitting the data, and resets fields to their default settings. You will use these buttons in the forms you create in this lesson.

  
**Radio buttons**

Radio buttons are never used as stand-alone items. They are reserved for two or more mutually exclusive options. To ensure exclusivity, a group of radio buttons must share the same _name_ attribute, although they will each use an individual value. The following example code shows two buttons representing mutually exclusive answers to the same question.

Should we add you to our mailing list? <br>

<input type="radio" name="AddToList" value="yes" checked="checked"> Yes

<input type="radio" name="AddToList" value="no"> No

![](https://srm--c.na127.content.force.com/servlet/rtaImage?eid=ka03x000000lhCR&feoid=00Na0000009SdkY&refid=0EM3x000003g11l)

**Check boxes**

Check boxes are used for a group of non-exclusive choices. You have two options when naming check boxes, and the option you choose depends on how you plan to use the collected data. Consider the following scenario. You want a list of the user's favorite hobbies. You plan to store the user's selections in a database. Are you going to store the user's entire response, which might include multiple hobbies, in a single field? Or do you want each hobby stored in a separate field in the database? Your choice will affect how you name the fields. In the next lab, you will see the results from both options.

The syntax for creating a check box is as follows:

<input type="checkbox" name="groupName">

As with radio buttons, you can preselect check boxes by adding the attribute _checked_="checked" into the tag. Unlike radio buttons, however, you can preselect as many check boxes as you like because check boxes are non-exclusive.

The following code will create a check box section on a form:

How did you hear about Amazon? (check all that apply):<br>

<input type="checkbox" name="ad"> Online Advertisement<br>

<input type="checkbox" name="friend"> From a Friend<br>

<input type="checkbox" name="convention"> Trade Convention<br>

The tags could also be written as follows:

<input type="checkbox" name="Origin"> Online Advertisement<br>

<input type="checkbox" name="Origin"> From a Friend<br>

<input type="checkbox" name="Origin"> Trade Convention<br>

With this syntax, each choice is treated as part of a single database field named _Origin_. Either method is acceptable, but one will be more appropriate depending on how you plan to use the data.

  
**Select Lists**

Select lists are drop-down lists of predetermined options. Depending on the settings, these lists can allow single or multiple selections.

#### **Single-option select list**

The syntax for creating a drop-down single-option select list is as follows:

<select name="listName">

<option>Option 1 </option>

<option>Option 2 </option>

...

<option>Option n </option>

</select>

The value that is passed when the form is submitted is the text to the right of the <option> tag. However, if you want to pass a value different from the text that appears in the list, you can add the _value_="" attribute into any or all of the <option> tags. In the next lab, one option will be set to pass a value different from the one the user will see.

In the following lab, you will add a single-option select list to the Web form. Suppose you want your model form to demonstrate a drop-down list of choices from which users can choose one. A select list provides this capability, and it is a form field type familiar to most Web users. You consider that the marketing team will want to contact candidates via email regularly, so a select list might provide an effective way to learn how often the candidates want to be contacted. How else might this type of list help the marketing team perform tasks?

### Multiple-option select list

Within the <select> tag, you can include the _multiple_ attribute as follows:

<select name="work" multiple="multiple" size="4">

The presence of this attribute automatically changes the select list to allow users to select more than one option. Because multiple selections are possible, these lists are usually presented with several, if not all, options already exposed.

The _size_ attribute of the <select> tag controls the number of items that will appear in a scrolling list box. If no size is specified, the number of items that will appear by default depends on the browser.

In the following lab, you will add a multiple-option select list to the Web form. Suppose you want your model form to demonstrate a drop-down list of choices from which users can choose one or more. A select list provides this capability, and it is a form field type familiar to most Web users. You consider that uCorp might need to know what time during the day to contact someone, so a select list might provide an effective way to learn when they are most respective to outreach. To facilitate scheduling, you should know all the times of day a  person is available, instead of limiting his or her choices to just one.

  
**Scrolling text area box**

You can use a text area box to gather more than one line of text from a user. The <textarea> tag provides a scrolling text box into which a user can enter a few sentences, an address, a letter to the editor or other text.

The <textarea> tag is a container tag, and the only content this tag can contain is text. Text between <textarea> tags will appear as default text within the box.

The <textarea> element has several key attributes, which you should understand and use. The following table describes these attributes and accepted values.

**Attribute**

**Description**

**Value**

**cols**

Specifies the width in characters of the scrolling text box.

Integer value (e.g.,

"25",

"40")

**rows**

Specifies the number of rows of text to display in the box.

Integer value (e.g., "2", "5")

**wrap**

Specifies whether user-entered text can wrap to new lines when submitted. This advanced attribute is used in conjunction with server-side scripts (such as PHP) that process form data.

If "soft" is specified, text in the textarea is not wrapped when submitted. This setting is the default.

If "hard" is specified, text in the textarea will wrap (adding newline characters) when submitted. The cols attribute must be specified when using wrap="hard".

_Note: The wrap attribute was deprecated in HTML 4.01 but was revived in HTML5 with "soft" and "hard" values, instead of the similar "none" and "virtual" values._

"soft" or "hard"

###   **Web Forms and CAPTCHAs**

To reduce spam submissions sent to your form, consider the use of a CAPTCHA (Completely Automated Public Turing Test to Tell Computers and Humans Apart). A CAPTCHA is a challenge-response mechanism designed to discern between a human and a "bot" in order to detect the automated systems used by spammers for registering email accounts.

A CAPTCHA is an automatically generated image presented to a user who has just submitted information or made a request of a Web server. CAPTCHAs require the user to view the distorted text image, and then enter the text shown in the graphic into a form field before he or she is allowed to proceed with a transaction. The distorted image is easily recognizable by humans, but is a difficult challenge for a machine. When the user provides the correct response to a CAPTCHA, then his or her input is accepted for processing.

CAPTCHAs can also require a user to view an image and identify each quadrant in which a specific object appears in that image.

Many CAPTCHA services exist, including:

###   **Search Engine Optimization (SEO) and Web forms**

When creating Web forms, you should take search engine optimization (SEO) into consideration. SEO involves learning how a particular search engine (such as Google, Yahoo! or Bing) ranks a Website. You can use this knowledge to customize a site's Webpages — including the forms used — so that the site is ranked as highly as possible in a search engine's results.

When conducting SEO, consider the following strategies related to forms:

-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)Create as simple a form as possible. Each additional field you use may reduce your score.
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)Some search engines may score pages lower if a CAPTCHA is used. The problem with a CAPTCHA, or any other element that requires human input, is that a bot that encounters it will not take time to read and process all of the page. This can cause the page to be scored lower.
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image052.png)Give form fields informative, descriptive labels.
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image053.png)Provide a clear call to action. Do not assume that a Submit button will inform users (or search engine bots) about what they should do.
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image054.png)Provide alternative text navigation.

**Case Study: In Good Form**

Lola works on the Web development team for her college. She has been assigned to create a Web form that will help the Language Department faculty plan a student trip to Europe in the summer. The faculty advisors want to use the Webpage to register interested students, collect itinerary suggestions, and gather information that will help them plan the travel accommodations. Lola's form needs to collect the following information from each interested student:

-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image056.png)Gender Languages studied
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image055.png)Preferred countries to visit Hotel room preferences
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image053.png)Student limitations related to physical abilities, diet, allergies, religious practices, etc.

![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image057.png)Lola decides to use the following form elements: Radio buttons to indicate gender

-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image012.png)Check boxes to indicate languages studied
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image011.png)A scrolling text area box to indicate preferred countries
-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image054.png)A drop-down select list to indicate hotel room preferences A text box to indicate student limitations

Lola posts the Web form on the Language Department page of the college Website. She then asks the department faculty members to review the form and let her know if they need any other information from students.

As a class, answer the following questions:

-   Did Lola use the correct form fields for the information requested? Why or why not?

Every form field was correct other than the preferred countries scrolling text area box implementation. It would be more efficient to display the preferred countries section as a drop-down select list or with check boxes. This would make the data more accurate and easier to measure due to the removal of potential human error in spelling and forgetfulness of potential countries.

-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image058.png)What other form fields could be used for the information requested on this form?

Aside from the form field implementations listed above, you could also use a scrolling text area to list student limitations. Many of these fields already listed have alternatives that could work just as well. Students can get creative here.

-   ![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image017.png)What other types of information might the faculty members ask Lola to collect for this project? Which form fields would work best for each new type of information? Why?

Lola may also be asked to collect data on what dates students will be available for the trip. One form field that would work for this are checkboxes that each cover a range of dates. Students would select every checkbox corresponding to dates they can go on the trip. Students can get creative here.

## Application Project![](file:///C:/Users/Joy/AppData/Local/Temp/msohtmlclip1/01/clip_image059.png)

Web forms are useless unless you can process them. Traditionally, the most popular way to process a form is through the use of a Perl-based CGI script on a Web server. However, many alternatives to Perl-based CGI have emerged. Alternatives include Active Server Pages (ASP), JavaServer Pages (JSP) and PHP Hypertext Processor (PHP).

Visit several Websites that use forms. View the Web form source code. Can you determine where the form is processed by viewing the element, and the _method_ and _action_ attributes?

###   **Skills Review**

In this lesson, you learned to use each of the major form field elements, and you created a functional Web form. You also saw the different form results that can be returned by setting the form action to point to a public test engine. You can test your knowledge after class by creating a form within a table in a new page.

### **Glossary**

  
**Client-side Script**

Code embedded into an HTML page and downloaded by a user; resides on the client and helps process Web form input. Common client-side scripting languages include JavaScript and VBScript.

**Common Gateway Interface (CGI)**

A program that processes data submitted by the user. Allows a Web server to pass control to a software application, based on user request. The application receives and organizes data, then returns it in a consistent format.

**Server-side Script**

Code that resides on a server to help process Web form input. Server-side CGI scripts are commonly written in Perl.