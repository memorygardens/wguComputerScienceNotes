You are not limited to HTML when developing Webpages. There are also client-side and server-side Web technologies for extending the capabilities of your Webpages. These technologies include:

-   Client-side and server-side scripting
-   Document Object Model (DOM) and Dynamic HTML (DHTML)
-   HTML5 Application Programming Interfaces (APIs)
-   Web application frameworks
-   Databases
-   Other advanced technologies made possible through the combination of HTML5, JavaScript, and Cascading Style Sheets (CSS3)

## Server-side and Client-side languages

Server-side and client-side languages are critical to extending the functionality of HTML. If you are interested in pursuing a career in Web development, or if you want to create Web apps for mobile devices, you should know how to use these technologies. You will probably be using these languages in the future.

### Basic programming terms

Before you learn about specific server-side and client-side languages, it is helpful to understand some basic programming terms.

CONCEPT

DESCRIPTION

**Variable**

A place in memory used to store information for later use. Variables

are used in simple applications and are essential in complex ones.

Variables are usually created by using the equal sign ( = ). For

example, to create a variable named David, you would use the

following command: David=David. Variables are often referred to as

values preceded with a dollar sign ( $ ). For example, the variable

named David would be referred to as $David. In many languages,

variables are case-specific (e.g., the variable $David is different from

the variable $david).

**Array**

A collection of variables stored in a series. Arrays are used to hold multiple values; a variable can hold only one value.

**Function**

A line of code that allows you to refer to an entire series of steps or

commands. Functions are used to organize code into discrete

sections.

**Interpreter**

Software used to read and process code in standard text files.

Interpreters either reside on the server or are downloaded to a client.

PHP, Perl and ASP are all languages that use an interpreter. Some CGI

applications must explicitly specify the location of the interpreter. For

example, Perl requires the first line to include a correct reference, or

the script will fail.

**Compiler**

An application used to process code in standard text files into

executable applications. For example, to compile a C application

named david.s, you would use the gcc application: gcc david.s -o

david.exe.

### Programming Statements

Even relatively simple scripts need to control the way that information flows within them based on conditions. Here, we describe several programming statements that allow applications to process information.

STATEMENT

DESCRIPTION

**If / then**

Executes a process only if a particular condition is true. For example,

an application may contain a statement that checks whether the

\tmp\ folder is present. If it is, then the application will run. Classic

if/then statements allow only one condition to occur. Known as a

conditional statement.

**If / then / else**

Similar to an if/then statement, but executes a group of additional

commands if the given condition is false. For example, an if/then/else

statement can direct the following logic: If the \tmp\ folder is not

available, then check to see if the \temp\ directory is available, or

else create a directory named \tmp\. Known as a conditional

statement.

**Do while**

Runs ("do") a specified subprocess while a specified condition is true.

For example, an application may continue to present an alternative

window while the mouse is being right-clicked. Often used as a part

of an if/then or if/then/else statement, the do while statement ensures

that an action occurs the entire time a condition is true. Sometimes

known as a repeat until statement.

**Do until**

Similar to a do while statement, but runs the specified subprocess

until a specified number of events have occurred. For example, a

calculation process may add the number 1 to the result of the

previous statement until the sum reaches 100, then exit.

**Break**

When placed inside of a statement, allows an application to break

out of an infinite loop in case of a problem.

### Server-side Languages

A server-side language has the following attributes:

-   Code is executed by the Web server, not by the Web browser.
-   Code is generally placed into files called applications. These applications are assigned execute permissions by the Web server. In some cases, code is embedded into HTML pages.
-   Code executes because an interpreter has been installed and activated on the Web server.

Server-side scripts are used for various purposes, including:

-   Browser detection
-   Database connectivity
-   Cookie creation and identification
-   Logon scripts
-   Hit counters
-   File uploading and downloading

Common server-side languages included PHP, Perl, Active Server Pages (ASP), Visual Basic, Python, C# and Java.

-   **PHP** - an interpreted server-side scripting language for creating dynamic Webpages. It is embedded in HTML pages but is always executed on a Web server.
-   **Practical Extraction and Report Language (Perl)** - a cross-platform programming language that enables users to write custom CGI programs and system management programs. Perl is a language commonly used for various purposes, including Web server processes.
-   **Active Server Pages (ASP) using VBScript** - Microsoft's original server-side scripting solution. It has largely been supplanted by .NET. You can create ASP applications using VBScript, which is quite like JavaScript, except that VBScript is a proprietary Microsoft language. PHP is an alternative to ASP.
-   **Python** - a programming language that was developed in the 1980s, but only started to gain popularity in 2004. It is touted for being easy to use. Python is object-oriented and has a plethora of frameworks that makes it more flexible than other languages.
-   **Go** - often called Golang, is a programming language developed by Google. Announced in 2009, and dropping its 1.0 release in 2012, Go is a relative newcomer in the world of programming languages.
-   **Java** - an object-oriented programming language. Java is a compiled language. However, unlike most compiled languages, Java is designed to allow its applications to run on any operating system that has the Java interpreter installed.
    -   **JavaServer Pages (JSP)** - JSP is a technology that uses Java commands embedded into HTML code.
    -   **Java servlets** - an application that must be installed directly onto the remote server; code from a Java servlet is not downloaded to the browser.
-   **Visual Basic** - compiled programming language developed by Microsoft Corporation. It is used for stand-alone applications and server-side Web applications. It is not often used as a client-side application in Web browsers, as is JavaScript or VBScript.
-   **C#** - (pronounced "C sharp") is a compiled object-oriented programming language and is the proprietary Microsoft competitor to Java. C# was designed to be easier to use (like Visual Basic) but still powerful.
-   **Server-side includes (SSIs)** - an instruction within an HTML page that directs the Web server to perform an action. SSI is considered to be an alternative to CGI because it does not use languages such as JavaScript, Visual Basic or Java. Rather, SSI instructions are written in SGML.
    -   **SSI file name extensions** - A Web server that supports SSI reads each HTML page for SSI instructions, and then processes the instructions for each user request. Standard practice is for HTML files that use SSI to use the .shtml or .shtm file name extension, rather than simply .html or .htm.
    -   **SSI support in Web servers** - Most Web servers include SSI capability. However, the SSI feature may be disabled. For example, if you are using Apache Server, you must edit the httpd.conf file to enter the instructions necessary for Apache Server to process the server-side includes found in HTML pages. With Microsoft Internet Information Services (IIS), you must select features in the GUI to enable SSI.

### Client-side Languages

Client-side languages run on the user's computer after the page is downloaded. Therefore, some of the processing burden can be passed from the server to the client machine. Using server-side technologies is sometimes preferable because there are risks inherent in allowing the client to determine the way your Webpages render. Consider the following problems:

-   Some clients do not support JavaScript or any other scripting language.
-   Users can deactivate script execution in browsers that normally support it. Many companies direct their employees to disable scripting in their browsers due to security concerns. If your page relies upon client-side scripting for browser recognition and/or database connectivity, then your pages may not render as expected to some portion of your audience.
-   User agents such as Lynx often do not support JavaScript or other forms of client-side scripting.

Netscape Corporation started developing LiveScript in late 1995. In early December 1995, just before Netscape Navigator 2.0 was released, Netscape and Sun announced that LiveScript would be known as **JavaScript**. The name was changed mainly for marketing purposes.

-   **JavaScript** - an object-based scripting language that allows developers to add interactivity to their Webpages. JavaScript can be used on the client side or on the server side.
    -   **JavaScript is object-based, not object-oriented** - JavaScript is not considered an object-oriented language because it does not support inheritance.
    -   JavaScript is an object-based language that has a collection of built-in objects, including:
        -   **Document** - allows you to obtain values from and write values to a document.
        -   **Navigator** - allows you to determine the type of browser accessing a Webpage.
        -   **Array** - allows you to create a series of variables to later manipulate.
        -   Several additional objects exist. JavaScript allows you to apply methods to all objects. For example, the document.write command in JavaScript allows you to write a specified value to a document.

ADVANTAGE

DESCRIPTION

**Quick development**

Because JavaScript does not require time-consuming compilation,

scripts can be developed in a relatively short period of time. Most

of the interface features, such as forms, frames and other GUI

elements, are handled by the browser and HTML code, further

shortening the development time. JavaScript programmers do not

have to create or handle these elements of their applications.

**Easy to learn**

Although JavaScript shares many characteristics with the Java

programming language, the JavaScript syntax and rules are

simpler. If you know any other programming languages, it will be

easy for you to learn JavaScript.

**Platform-independence**

Like HTML, JavaScript is not specific to any operating system. The

same JavaScript program can be used on any browser on any

system, provided that the browser supports JavaScript.

-   **External JavaScript** - JavaScript can also reside in external files with the .js file extension. These external files are useful when the same JavaScript code needs to be repeated in many different Webpages. It will keep each of these pages less cluttered, as well as help maintain consistency between pages.
    -   The downside to using external JavaScript is that, when the JavaScript is small, it can slow down the Webpage compared to embedded JavaScript. This is because the HTML page will need to take an additional step in requesting the JavaScript from the Web server every time it is loaded.
-   **JavaScript and cookies** - You can also use JavaScript to deposit cookies on the system hard drives of users who visit your site.
-   JavaScript can also be used for **copyright protection**. A simple script can help prevent your Website from being included in another site without proper recognition.

## Dynamic HTML (DHTML)

Dynamic HTML (DHTML) is an umbrella term to describe HTML's ability to work with other technologies to provide animation, interactivity and dynamic updating in Webpages. With DHTML, you can create a Webpage that reacts to user actions without contacting the server or downloading complex, bandwidth-consuming applications. Because it eases the burden on the server, DHTML is an effective front-end and back-end solution.

### Document Object Model (DOM)

The **Document Object Model (DOM)** is a standard developed by the W3C. It describes the elements, or objects, within a document rendered by a Web browser. It is a vendor-neutral, cross-platform Application Programming Interface (API) that specifies how objects in a document can be referred to and manipulated through scripting languages.

To work with the DOM for any browser, you need to use a scripting language, such as JavaScript or VBScript. JavaScript is more difficult to learn, but more universal.

[For more information about the DOM and for a visual example, visit W3schools](https://www.w3schools.com/whatis/whatis_htmldom.asp).

### HTML5 API

The future of Web development will probably focus on HTML5 APIs. They provide an open environment for developing Web applications that does not rely on proprietary browser plug-ins. The HTML5 APIs are an excellent example of DHTML.

HTML5 APIs consist of HTML5, CSS3 and JavaScript. JavaScript is used to access the DOM. These technologies used together create webpages that can easily adapt to smartphones, tablets, gaming devices and smart TVs, as well as to traditional PCs.

For a complete list of HTML5 APIs from one of the W3C members, visit [http://platform.html5.org/](http://platform.html5.org/).

-   **Canvas** - an HTML API that provides a place on a Webpage (a "canvas") where developers can display graphics, animation, video and games "on the fly" without the need for a plugin.
-   **Offline Web applications** - allow users to interact with Websites while they are offline. This will allow a user to continue to interact with a Website when a network connection is unavailable. Webpages will store data locally within the user's browser, utilizing the application cache, allowing them to continue accessing the site.
    -   Utilizing a **manifest**, which tells the browser which files to store locally, is what allows the user to continue working without the connection. When the user goes back online, the application cache will automatically update when revisiting the Website. The application cache will reload that file in the event any of the existing data has changed in the cached files.
-   **Geolocation** - determines how to display a user's location based on how the user visits a Website. A number of technologies can be used, such as the user's IP address, wireless network, or GPS hardware utilized on his or her device.
-   **Drag-and-drop** - allows a user to move an item from one place on the page to another by dragging it across the screen and dropping it in a different location.

## Web Application Framework

A **Web application framework** is a software framework that enables developers to create and manage dynamic Websites, Web applications and Web services. Software frameworks generally provide common programming code for generic functions that can be selectively overridden by the developer for specific functionality.

There are two types of frameworks, frontend and backend. Frontend frameworks have features that help developers create a dynamic, elegant, and interactive user experience from a design and functionality standpoint. Current frontend frameworks include Angular, React, JQuery UI, and Vue.js. Backend frameworks focus on controlling data access, storage, and manipulation of data through RESTful API services, WebSockets, caching, and other data centric technologies.

Two Web application frameworks that are quickly gaining favor with Website developers are:

-   **Django** - an open-source Web application framework that is designed to support the development of dynamic Websites.
-   **Ruby on Rails** - another open-source Web application framework that also emphasizes Rapid Application Development (RAD) and the Don't Repeat Yourself (DRY) principle for rapid Website development.

### Connecting to a Database

For a database to work, you must:

-   Provide a way for the Web server and database to recognize each other
-   Provide permissions to the database so that it can be read and/or written to

### ISP AND WEB SERVERS

If you are working with an Internet Service Provider (ISP), you generally need to request a Web server. Following are the actions you will need to request that the ISP perform:

-   Enable execute permissions on your scripts
-   Create a directory that contains available scripts
-   Provide user names and passwords with enough permissions for the system

### N-Tier Applications

When discussing databases, three elements are generally involved:

-   **Data** - the database file or multiple database files.
-   **Business logic** - the SQL coding necessary to create relationships with the data stored in the database.
-   **Presentation** - the way that data and business logic are presented on the user screen. Presentation includes Web forms created with HTML, and application-specific interfaces such as Microsoft Access or a Web browser.

In a single-tier database, the data, business logic and presentation are all provided by one application (e.g., Microsoft Access). In a two-tier application, the client is responsible for the business logic and data presentation, and the database is stored on a separate server. In an n-tier solution, all three database elements are separated.

![[Pasted image 20220615233431.png]]