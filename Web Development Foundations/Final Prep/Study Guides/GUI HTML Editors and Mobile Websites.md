A Graphical User Interface or GUI editor allows web developers to quickly create a webpage without the need of manually typing HTML or CSS. GUI editors are also known as What You See Is What You Get (WYSIWYG) editors.

# Text Editor vs. GUI Editor

![[Pasted image 20220615233544.png]]


# The W3C Authoring Tool Accessibility Guidelines (ATAG)

The ATAG specifies guidelines for GUI editors to ensure accessibility for all developers. The guidelines are broken into two parts: A & B. Part A addresses the UI while Part B addresses the production of accessible content. The following is from the [W3C.org](https://www.w3.org/WAI/standards-guidelines/atag/glance/).
![[Pasted image 20220615233802.png]]

# HTML Validation

The W3C provides a way for you to check your HTML files for syntax errors at [https://validator.w3.org/](https://validator.w3.org/)

The following information about Markup Validation is from the [W3C.org](https://validator.w3.org/docs/help.html#validation_basics):

#### What is _Markup Validation_?

Most pages on the World Wide Web are written in computer languages (such as HTML) that allow Web authors to structure text, add multimedia content, and specify what appearance, or style, the result should have.

As for every language, these have their own _grammar_, _vocabulary_ and _syntax_, and every document written with these computer languages are supposed to follow these rules. The (X)HTML languages, for all versions up to XHTML 1.1, are using machine-readable grammars called DTDs, a mechanism inherited from [SGML](https://validator.w3.org/docs/sgml.html).

However, Just as texts in a natural language can include spelling or grammar errors, documents using Markup languages may (for various reasons) not be following these rules. The process of verifying whether a document actually follows the rules for the language(s) it uses is called _validation_, and the tool used for that is a validator. A document that passes this process with success is called _valid_.

With these concepts in mind, we can define "markup validation" as the process of checking a Web document against the grammar (generally a DTD) it claims to be using.

# CSS Validation

Likewise, the W3C also provides a way for you to check your CSS files for syntax errors at [https://jigsaw.w3.org/css-validator/](https://jigsaw.w3.org/css-validator/)

# Website Publishing

The final step in Website development is publishing your site to the World Wide Web. You can publish your site in several ways, depending on the tools used to create it. Most GUI HTML editors provide a Publish feature that allows you to easily post your Webpage files to your designated Web host. You can also use a File Transfer Protocol (FTP) client, such as FileZilla (http://filezilla-project.org/).

### Publishing to a test Web Server

FTPis the protocol most often used to transfer files between two computers, or a server and a computer, depending on the configuration. Transferring files over the Internet requires an FTP client to send the files and a destination FTP server to receive them. FTP can also be used to transfer files to an HTTP server, provided that the HTTP server is also running FTP. However, before you can transfer your Website files, you must decide where your site will be hosted. Professional Web developers post the final version of the Website files to a test Web server before moving them to the production server for the following reasons:

-   To verify that the Web server can process any CGI and database access requests.
-   To locate and repair any dead links.
-   To allow members of the development team and other stakeholders to preview the site. You will find that many changes are needed before your "final" code is ready for publication.

### **Test Server Configuration**

Your test server must be as nearly identical to the production server as possible. The test

server should have:

-   The same operating system version — If your production server is a Linux system or a Windows Server, for example, then your production system should be the same model.
-   The same type and version of Web server software — Even if your test system uses a software type or version very similar to the production system, this test system is not adequate. For example, if your production Web server uses Apache Server 2.2 and your test server is using Apache Server 2.4, then your testing server will not provide a true test of your site.
-   The same CGI interpreter software — If your production server uses PHP 5.4.0, then your test server should use PHP version 5.4.0.

# Designing Websites for Mobile Devices

The use of mobile devices has increased significantly over the past 10 years. This [article from Pew Research](https://www.pewresearch.org/internet/fact-sheet/mobile/) (April 2021) shows that 97% of Americans own a smartphone.

According to [Statista](https://www.statista.com/statistics/277125/share-of-website-traffic-coming-from-mobile-devices/), mobile devices account for more than 50% of website traffic (as of first quarter 2021).

The following are suggestions for optimizing your website for mobile devices:

-   Keep pages simple and uncluttered.
-   Prioritize your content. Provide the most essential content first.
-   Optimize your website for smaller screens.
-   Include a meta viewport tag and use responsive web design.
-   Ensure that your HTML and CSS pass validation.
-   Separate your content and design. Use external style sheets and avoid internal and inline styles.
-   Include the alt attribute within all <img> tags.
-   Include labels for all form fields.
-   Use consistent heading elements (h1 – h4). Avoid smaller heading elements.
-   Use 100% of the screen space. Specify less margins and padding in CSS.
-   Navigation should be intuitive.
-   Ensure that your content is easy to read on a mobile device.

### **Mobile Apps vs. Mobile Websites vs. Responsive Web Design**

There are many arguments regarding the better approach for mobile devices: mobile apps, dedicated mobile Websites or responsive design Websites. Mobile apps are stand-alone applications that are downloaded from a vendor's software repository onto a mobile device. Apple iTunes and Google Play are two leading providers of apps for the Apple and Android mobile devices, respectively. As you have learned, mobile Websites are usually strippeddown versions of traditional Websites.

### Responsive Web Design (RWD)

Websites that use RWD  are normal Websites that are designed to function properly and seamlessly on all screen sizes and resolutions. For HTML5 developers, the difference is fading between mobile apps, mobile Websites and responsive design Websites. Opportunities exist in these arenas because HTML5, CSS3 and JavaScript are now being used to create both mobile apps and Websites.

Open [nasa.gov](https://www.nasa.gov/) in Google Chrome and use [Chrome's emulator](https://www.browserstack.com/guide/view-mobile-version-of-website-on-chrome) to view the website with a mobile viewport, tablet viewport, laptop viewport, and desktop viewport. 

# AJAX

AJAX stands for Asynchronous JavaScript and XML. Simply put, AJAX allows the user to load new page content without the need of loading a new page. Instead, new content can be loaded within the same page using AJAX and an XMLHttpRequest (AKA XHR).

For more information about AJAX and how it works, visit [w3schools.com](https://www.w3schools.com/php/php_ajax_intro.asp).

# Web 2.0

Web 2.0 is a paradigm shift in the way the Internet is used compared with the Web 1.0 day. Web 2.0 involves a more open approach to the Internet that concentrates on developing the information-sharing and collaboration capabilities of the Web. Web 2.0 has enabled users to provide a significant amount of information on the Web, and there are no longer any restrictions on what they produce. Web 2.0 has also led to the development of Web-based communities and hosted services, such as social networking sites, video-sharing sites, wikis, blogs, RSS feeds, podcasts and so forth. The Web is now a resource through which users have the ability to generate and distribute content, as well as to update and modify it.

Examples of Web 2.0 include: Facebook, Twitter, YouTube, etc.

# Web Feeds

A web feed is a data format used to provide frequently updated content. Examples include news feeds, YouTube channels, Twitter feeds, podcasts, and blog posts. Common formats include Really Simple Syndication (RSS), JavaScript Object Notation (JSON), and Atom.

# Cloud Service Providers 

Traditional cloud hosting service providers offer complete Website solutions. These solutions include a Web domain, Web server space, Website building tools, Website security and bandwidth. 

Cloud service providers, such as Amazon Web Services, Microsoft Azure and Google Cloud are prepared to provide more complete services, including but not limited to:

-   **Software as a Service (SaaS)**, such as email, accounting, human resources management, customer-service relationship, Web hosting, and nearly any type of software.
-   Infrastructure as a Service (IaaS), such as virtual machines, firewalls, IP addresses and computing infrastructure. Backup services and nearly unlimited hard drive space on a pay-as-you go subscription.
-   Advanced Web and database connectivity, including the creation of custom CGI applications. Advanced Web development and machine learning tools.
-   Enterprise resource planning (ERP), which is the ability to automate the planning and operations of your entire organization (e.g., hiring, termination, manufacturing, marketing).