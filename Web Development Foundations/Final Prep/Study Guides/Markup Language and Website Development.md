# Introduction

## MarkUp Language

It is important to understand that Webpages are no longer viewed only through standard Web browsers. Your smartphone, tablet, smart TV and gaming console are all capable of reading **markup languages**. In fact, many Web design professionals refer to HTML as "markup," simply because many of their pages will be viewed using applications other than traditional desktop Web browsers. Many Web design professionals now design sites using **responsive design** principles, that enable a Website to be dynamic and accessible on every sized device available. Responsive design includes practices like defining sizes in percentages rather than absolute pixels, and checking device specifications to deliver one of multiple style sheets that best fit the user's needs. Because markup languages are becoming more common in the workplace, it is important for you to understand how to use them.

Webpage creation by any method requires a working knowledge of **Hypertext Markup Language (HTML)**. It is the standard markup language on the Web, and in other settings. HTML is standardized by an organization called the World Wide Web Consortium (W3C). You can learn more about the W3C at [_www.w3.org_.](http://www.w3.org/)

HTML is the markup language that defines page structure, hyperlinks, graphics and more to enable pages to render in Web browsers and other devices. You will learn about HTML in detail throughout this course. You can type HTML code manually into a text editor, use a graphical user interface (GUI) editor program to create the code automatically (by pointing and clicking your mouse), or combine both methods.

### HTML Versions

HTML 5.2 is the latest verion.

HTML 3.2 is an older but functional HTML standard. Some Webpages and HTML editors still use the 3.2 and 4.01 standards.

The HTML 4.01 Recommendation (released in 1999) contained many improvements from HTML 3.2, most notably Cascading Style Sheets (CSS). You can access this standard at [_www.w3.org/TR/html4/_.](http://www.w3.org/TR/html4/) The 4.01 specification included minor modifications to the 4.0 specification.

HTML 4.01 supported multiple spoken languages. For example, HTML 4.01 allowed you to create Webpages that read languages such as Hebrew from right to left. HTML 4.01 also allowed you to create ambitious tables and forms, as well as incorporate scripting languages. You will learn more about scripting solutions, such as JavaScript, later in the course.

As Webpages were developed in HTML 4.01, they had three distinct variants, or "flavors." The HTML 4.01 flavors ensured that you could use the specification and still remain backward-compatible with older Web browsers. Following is a short description of each flavor.

-   **HTML 4.01 Transitional** —allowed developers to insert formatting using either CSS or traditional layout instructions (e.g., HTML font, color and phrase elements). This version rendered in browsers that did not support HTML 4.01 features such as CSS. This version also allowed tags that the W3C considered to be less useful, known as "deprecated tags."
-   **HTML 4.01 Strict** —required the exclusive use of CSS when defining layout instructions. Deprecated tags were not allowed and generated errors.
-   **HTML 4.01 Frameset** — required for pages that used HTML frames, which placed Webpages inside each other to create separate panes in the browser window. Some felt that frames provided additional functionality or enhanced a site's look and feel.

[Visit W3Schools.com, HTML History, for a closer look at HTML versions](https://www.w3schools.com/html/html_intro.asp). 

### XML

**Extensible Markup Language (XML)** is a language used to describe data elements on a Webpage. XML enhances the structure and navigation of data. It is not used to format the page's appearance. Businesses use XML because it allows data to be interchanged with all types of applications.

XML is often used with intranets and extranets because these systems tend to focus mostly on sophisticated personal and business transactions. These types of transactions require the elements that XML offers.

XML documents can be formatted into print documents, Web documents, PDF documents, comma-separated values (CSV), Braille, text-to-speech and many other formats. This versatility allows XML to easily format content from a textbook, for example, which can be published to the Web in an e-learning course. Because the documents are well-formed and define only the content, changes can occur on the fly (i.e., dynamically or without interruption), without administrators or programmers manually reformatting the content before transmission.

XML is often misunderstood. Many people think XML is just another set of markup used to format Webpages. This assumption is incorrect. In fact, XML is not used to format Webpages, but to describe the data from which Webpages are created. The W3C governs the development of XML.

### HTML5

HTML5 provides modern requirements for the Internet with fewer plug-ins, such as the ability to standardize how video and audio are presented on a Webpage. To that end, HTML5:
-   Introduced the <video> element, which is designed to eliminate the need to install third-party plug-ins (such as those for Adobe Flash or Microsoft Silverlight).
-   Adds the <audio> element, which allows pages to seamlessly add audio files for events such as podcasts.
-   Establishes ways to enable drag-and-drop capability for Webpages without using third-party add-ons. Gives developers more native tools such as download progress indicators, image captioning options and form validation tools to use on a page.
-   Provides developers with a native option for **offline storage**, and enables applications to run as expected even without network connectivity.
-   Allows developers to retrieve the geographical location information for a client-side device, called **geolocation**. Examples include using the Global Positioning System (GPS) of a mobile device to determine the device's location, which allows Web services to be provided based on the client's location.

You will learn more about HTML5 throughout this course. To view the HTML5 specifications, go to:

[_http://dev.w3.org/html5/spec/Overview.htm__l_](http://dev.w3.org/html5/spec/Overview.html)

### Markup Validation

It is possible to validate all markup code automatically. Many validators exist, but the most authoritative is the W3C Markup Validation Service (_https://validator.w3.org/_).

Using this service, you can upload local HTML files for validation, or provide the URL of a Webpage to validate it. In this course, you will use the W3C validation service to validate your HTML5 code. However, it is important to note that this validator reads the

<!DOCTYPE> declaration on an HTML page and validates according to the specified DTD. So, if your document references an older HTML 4.01 Strict DTD, then the validator will validate code according to the HTML 4.01 Strict specifications.

To reiterate, make sure you adopt a single W3C standard and apply it consistently so that when you validate your markup code, the code and your specified DTD will match, and the results of the validation process will be legitimate.

Validating your markup code is worthwhile because validated code is most likely to be interpreted accurately by the majority of user agents. As a result, your pages will render as you expect and will be available to a larger audience.

Following are some tips to consider when validating your markup code:

-   Do not be discouraged when you see multiple problems reported for a page. Sometimes one small flaw can cause the remaining code on the page to fail validation, even if the remaining code is actually valid.
-   When errors are reported, search through the code carefully to find the true problem. Sometimes when a validation program finds a problem, it does not report the correct cause or it may not report the cause clearly.
-   Make sure that you are validating the correct file.

## CasCading Style Sheets (CSS)

**Cascading Style Sheets (CSS)** are rules in an external text file that determine how to display HTML elements in your Webpages. CSS3 contain formatting instructions that can define the font, color and phrase elements used on a particular markup page.

Cascading style sheets is currently in its third version (CSS3).

If all pages on your site are linked to the same external style sheet, then one simple change to the style sheet will change all elements across the site. If you then want to change those instructions (for example, the size of a document heading), you need not change every page manually. You need only change a line in the style sheet file, then all your headings will change their appearance to conform to the style sheet. This technology can save a great deal of development and maintenance time, as well as make a more consistent, accessible interface.

You can validate CSS with the validator from W3C at: [https://jigsaw.w3.org/css-validator/](https://jigsaw.w3.org/css-validator/)

## Editors

To create a webpage, you need to use a text editor or a GUI editor. See information about both below.

### Text Editors

You do not need to use a special editor application to create HTML. You can use a simple text editor. A text editor is any program that allows you to type simple text and edit it, such as Microsoft Notepad and WordPad, or UNIX-based programs such as Vi and Pico. However, you must save your code files as plaintext. Any formatting instructions embedded in a file by a word-processing program, for example, can prevent the file from functioning properly.

After you save the Webpage code as a text file, you should save it with the .htm or .html file name extension. Many operating systems and Web browsers are configured with **Multipurpose Internet Mail Extensions (MIME)** to automatically process files with these extensions.

Many text editors exist, all with more capability than Microsoft Notepad. Open-source examples you may want to use include:

-   **Atom –** [https://atom.io/](https://atom.io/) (Windows, macOS, Linus)
-   **Cream** — [_http://cream.sourceforge.net_](http://cream.sourceforge.net/) (Windows only).
-   **Emacs** — [_www.gnu.org/software/emacs_](http://www.gnu.org/software/emacs) (Windows, macOS, or Linux).
-   **jEdit** — [_www.jedit.org_](http://www.jedit.org/) (Windows, macOS, or Linux).
-   **Notepad++** — [_http://notepad-plus.sourceforge.net_](http://notepad-plus.sourceforge.net/) (Windows only).
-   **Sublime Text** — _https://_[_www.sublimetext.com_](http://www.sublimetext.com/) (Windows, macOS, or Linux).
-   **Vim** — [_www.vim.org_](http://www.vim.org/) (Windows, Mac or Linux).

Most of these products have versions that will run on multiple operating systems.

### GUI Editors

**Graphical user interface (GUI)** markup editor applications place markup instructions into files for you; you do not need to know HTML to use GUI editors. Many GUI HTML editors still do not produce valid HTML. Nevertheless, such editors provide a graphical user interface that makes it easy for you to create HTML pages without writing any code manually. You simply point and click with your mouse, and the code is generated by the program. Commands are displayed on the graphical user interface as they will appear in a browser, thus the programs are often called WYSIWYG (What You See Is What You Get) editors. Some developers feel that using a GUI editor application saves time. Others feel that GUI editors create confused HTML code and do not provide true flexibility.

Popular GUI HTML editors include Adobe Dreamweaver, Microsoft Expression Web, Mozilla SeaMonkey and Google Web Designer.

For more information about text editors and GUI editors see [GUI HTML Editors and Mobile Websites](https://srm--c.na127.visual.force.com/apex/coursearticle?Id=kA03x000000l9NwCAI&). 

## The Web Development Trifecta: HTML, CSS, JavaScript

The future of Web design lies within three technologies: HTML, Cascading Style Sheets (CSS) and JavaScript. These technologies used together create websites that optimize for an array of devices, including smartphones, tablets, gaming devices and smart TVs, as well as to traditional PCs.

HTML5, CSS3 and JavaScript are sometimes called the "HTML5 family." The following table the functions of each technology.

**Technology**

**Description**

**HTML**

Markup language used for structuring and presenting Webpage content

**Cascading Style Sheets (CSS)**

Style sheet language that provides the formatting and "look" of a Webpage or document written in a markup language

**JavaScript**

Scripting language that provides dynamic, interactive capabilities to Webpages

## Web Development Project Cycle

Creating a Website requires you to work closely with individuals and teams of individuals. To work smoothly with other teams, you must carefully outline and communicate the project's steps. While you may not manage the project, at the very least you will be part of it. So you must understand the typical Web development project cycle. Consider the following steps:

1.  Create and document an initial Website plan.
2.  Obtain relevant input from stakeholders.
3.  Communicate the Website plan.
4.  Consider technical and non-technical concerns.
5.  Develop the website.
6.  Publish the website.
7.  Website maintenance.

### Website Plan

Before you can create any HTML code, you must first create a plan for the site. This plan has several names, including: Site diagram and Storyboard

Regardless of the name you use, this plan must include the following:

-   A statement discussing the purpose and intended audience for the site. This statement may evolve over time, but it is important to begin with this statement to remind everyone involved why the site is being developed and to steer all efforts in the proper direction.
-   A rough outline of the pages needed, including:
    -   The default page (e.g., index.html), also called the home page.
    -   Sections of the site (e.g., products, sales, international, contacts).
    -   An estimate of the technologies required (e.g., databases, Web servers, search capability, indexes).

Your Web team cannot create this plan in isolation. You must obtain input from stakeholders.

### Wireframe

**Wireframing** is another helpful tool for Website planning. Wireframing is the process of developing an outline for a Web presence. A wireframe is presented as a visual representation of a Webpage layout, as shown in [this example](https://balsamiq.com/assets/learn/articles/mobile-web.png). Wireframes usually focus on representing a Website's layout. Multiple wireframes can make up a storyboard, which will be discussed later in the lesson.

Steps in the wireframing process usually include:

-   Determining the purpose and objective of the Website. Is this an e- commerce Website? An informational Website? A company intranet? Identifying all stakeholders for the site.
-   Outlining the basic steps of the development process. Identifying steps for managing the project.
-   Outlining site navigation.
-   Identifying the technologies that are invoked with each user request.

As you can see from this list of tasks, quite a bit of work occurs before pages are created. Sometimes, software can help you with wireframing and project management.

### Stakeholder and Audience

Successful Websites have a strong, central theme aimed at a distinct audience. They have the ability to support this theme by providing clear explanations and related services. You must start with a strong message, then consider how this message will be presented. Even the best looking Webpage or site will fail in its purpose if it does not have a clear message.

As you determine your audience, consider eliciting input from various parties, including:

-   **Customer representatives** — Organizations often have important customers attend meetings and provide input. Customer representatives can teach you about the various types of messages that appeal most to potential customers. For example, some may want to focus on the value of a particular product, regardless of cost. In other instances, customers may help you focus on a message that shows your products to be inexpensive. Once you have surveyed customers to determine what the market wants, you can begin to craft Webpages that clearly convey your company's message to its intended customers.
-   **Suppliers** — If you are planning for large sales as a result of your Web effort, make sure that your product suppliers are ready for this. Otherwise, you could damage the company's reputation by making promises that cannot be kept. Even though a Web authoring team works mostly on creating markup pages, your Website's ability to communicate with the public means that such business concerns are essential for the overall success of the project.
-   **Shareholders**— If your organization is publicly owned, you may need to obtain input from shareholders about the look and feel of the site.

### Design Considerations

The design elements with which you display information on your site can be just as important as the information itself. As previously discussed, the front end you present to users may determine whether users remain at and return to your site. Consider the following design concepts:

-   **Message** — Deliver a coherent message for each page. Information that is not relevant or otherwise distracts readers from a well-conceived central idea should be placed on another page or eliminated.
-   **Fonts** — If specifying fonts, make sure that you use common ones so that browsers do not have difficulty rendering them. Use proper sizes; small fonts are difficult to read.
-   **Images** — Make sure that all images used on a page contribute to either the page's navigability or its message.
-   **Color** — Take time to consider color combinations so that your pages are as attractive and readable as possible.
-   **Language** **choice** — Some organizations will need to use only one language for their sites, such as English. Others may need to create multiple sites in various languages to accommodate an international audience. Still others may offer an immediate choice of one or two languages because the government of the country in which they reside demands such accommodations, for example.
-   **Common color schemes** — Preferences for color combinations differ from one culture to the next. Remain sensitive to and informed about such preferences.
-   **Messages that appeal to customers** — You may need to alter your message about a particular product or activity if you present it to another culture. Consider the expectations and preferences of specific cultures so that your message is as clear and appealing as possible

Validation should occur on a regular basis as the site is being developed. Although a final validation is necessary, the final validation should not be the only one.

### Stakeholder Input

When creating a Website, stakeholders are relevant organization employees or contributors who can provide or help determine the following information:

-   The purpose of the Website.
-   The site's look and feel.
-   The services that the audience requires from the site.
-   Budget
-   Timeline
-    Although your team will largely determine how long it will take to create the site, your team will also have to coordinate with other departments in the organization. For example, the sales and marketing teams are likely to have important input about when the site is published, as well as its look and feel.

### Storyboard/SiteMap

A storyboard or sitemap is a hierarchal depiction of the pages within your website. [See this example](https://images.template.net/wp-content/uploads/2015/08/Download-Printable-Website-Storyboard-Word-Format-Sample.jpg).   

### Website Plan Documentation

In addition to creating a site storyboard, you must also document decisions made in all meetings. All plans must be distributed and approved. Any decisions involving changes in dates and allocations of funds may require further approval from the organization.

### Technical and Non-Technical Concerns

In your meetings, you are likely to find that although everyone may share the same goal, they may not be able to communicate specific needs to each other. A common problem is that some team members do not have much technical knowledge, but nevertheless have ideas that are essential for the success of the site. Often, the non-technical employees in your meetings can ensure funding for your project.

It is the project leader's responsibility to ensure that input and requests from team members with little or no technical knowledge are heard and seriously considered. Similarly, you must ensure that project members with technical experience clearly convey their capabilities, limits and needs to non-technical team members. Otherwise, team members will constantly speak past each other, and confusion will result. Confusion can increase especially if project members work remotely. Ways to ensure clarity both in meetings and in communication include:

-   **Regularly asking if anyone has questions** — This strategy helps some team members speak up. However, less outgoing individuals who have questions may still hold back.
-   **Asking team members to summarize their understanding of decisions** — Although this strategy puts some people on the spot, this is preferable to having team members remain confused about the project's direction.
-   **Asking** **a** **third** **party** **to** **deliver** **a** **summary** **of** **progress** — This third party can attend your meeting and ask questions of team members. By listening to responses, you can gauge overall team participation and understanding.
-   **Writing regular updates about the project** — Make sure that in your updates you translate technical requirements into non-technical language, and vice versa.

### Developing the Website

Once you have obtained enough information and created a definitive plan, you can begin developing the site. As your team develops the site, you will be engaged in various activities, including:

-   **Creating markup code** — You will develop pages that fulfill all design standards.
-   **Testing functionality** — Make sure that the site performs well technically before it is published to the Web. This involves testing the site in multiple browsers, for example.
-   **Approving the site** — All stakeholders will need to approve your team's work. Make sure that all parties have seen the site before publication, and make sure that you have documented this fact.
-   **Publishing the site** — The site must be properly placed on a Web server. You may also participate in decisions such as whether you will configure your own Web server or use a Web server configured by another provider.

### Website Maintenance

You are unlikely to develop and post a site that never needs modification. In fact, managing a site usually requires more time and work than initially developing it. As part of a team that manages a site, you must:

-   **Create new content** — The perception that a site has failed to remain current can be damaging. Innovation and fresh content are both essential to managing a site that stays popular.
-   **Update** **dead** **links** — For various reasons, links that once functioned may fail over time. A link can become invalid because a page's location was changed on the hard drive, or because the link pointed to an external Website that no longer exists or has changed its structure. You can use automated applications to check your site for dead links. However, someone must still manually alter any invalid links to make them valid again.
-   **Remove old sites** — Sometimes an entire site becomes invalid. It is your duty to remove such sites from the Internet.
-   **Remove unused pages** — Pages on Websites sometimes become stale, especially if they are tied to a marketing campaign. If they cannot be updated, they must be removed.
-   **Ensure connectivity** — You or a member of the IT department may be assigned to ensure that the site is active and that enough bandwidth is available. You may have to upgrade or downgrade bandwidth, depending upon customer volume. You do not want customers to be frustrated by slow site access, but you also do not want to pay for unused bandwidth.
-   **Report access troubles** — Sometimes you need to contact your ISP and begin a **trouble ticket** to begin resolving a problem. It may also be your responsibility to follow up with problems to ensure they are properly resolved.
-   **Process feedback from customers and stakeholders** — Your team will be asked to make changes to the site periodically. Some changes may be subtle; others may require considerable effort on your part to make the site fulfill its potential and truly benefit your organization.

## Accessibility

This section addresses accessibility.

### Americans with Disabilities Act (ADA)

The Americans with Disabilities Act (ADA) was enacted in 1990 to protect the civil rights of disabled people. The ADA is a broad application of accessibility standards to influence commercial and social practices related to persons with disabilities. This law has many sections and includes mandates for equal employment opportunities and public accommodations for disabled people. It also includes mandates that electronic information be accessible to disabled people. Significant compliance failures are subject to financial penalties.

According to the U.S. Justice Department, the ADA also applies to cyberspace communications. In an opinion letter dated September 9, 1996 (_https://_[_www.w3.org/WAI/EO/EO-Policy-USDOJ_),](http://www.w3.org/WAI/EO/EO-Policy-USDOJ)) the U.S. Department of Justice stated the following:

"_Covered entities under the ADA are required to provide effective communication, regardless of whether they_ _generally communicate_ _through print media, audio media, or computerized media such as the Internet. Covered entities that use the Internet for communications regarding their programs, goods or services must be prepared to offer those communications through accessible means as well._"

Because it is an active law, the ADA is relevant to anyone designing pages in the United States, and anyone creating sites that will be visited by users who live in the United States. The standards are officially known as the U.S. Department of Justice ADA Standards for Accessible Design. Any penalties are the result of prosecution brought by the U.S. Justice Department; lawsuits from individuals and class action suits are not possible. The Justice Department tries to determine good-faith efforts before bringing lawsuits, and generally punishes only violators who exhibit long-term, wanton disregard for the standards. To learn more about ADA, visit _https://_[_www.ada.gov/_.](http://www.ada.gov/)

As a Web designer, your job is to create what the Department of Justice calls "reasonable accommodation" in your Websites for people with various disabilities. You must make reasonable accommodations if you are a covered entity, which according to ADA is any "private employers, state and local governments, employment agencies and labor unions". Critical ADA compliance factors to consider when creating reasonable accommodations in your Websites include:

-   Ensuring that all images have text-based descriptions so that sight-impaired visitors can access sites through screen-reader technology.
-   Providing text-based alternatives to all non-text content (e.g., Java applets). Providing forms that are easily read by screen-reading technology.

Video is not ADA-compliant because sight-impaired visitors cannot see it. Video with audio but no alternative text support is a problem because hearing-impaired visitors cannot hear it.

### Section 508 of the Rehabilitation Act

On June 21, 2001, the U.S. government implemented Section 508 of the Rehabilitation Act: Electronic and Information Technology Accessibility Standards. Section 508 requires that Federal agencies provide accommodations for users with disabilities for all electronic and information technology developed, procured, maintained or used by federal agencies. Section 508 is based on the Priority 1 and 2 checkpoints of the W3C's WAI Web Content Accessibility Guidelines 1.0. You can learn more about Section 508 by visiting the following URLs:

-   Federal Information Technology Accessibility Initiative, Section 508 home page (_www.section508.gov_)
-   U.S. Access Board, Section 508 of the Rehabilitation Act ([_www.access-board.gov/508.htm_)](http://www.access-board.gov/508.htm))

The chief purpose of Section 508 is to ensure that disabled individuals have a comparable level of access to information. Each standard aims to ensure that Webpage design and other computer-based elements do not limit access to information by disabled users. Section 508 includes the following standards for Websites:

-   All non-text elements must have a text-based equivalent.
-   If using multimedia, all equivalent information must be properly synchronized with the multimedia so that disabled persons are not at a disadvantage.
-   Information must be equally available in color and without color.
-   Documents must be made available without requiring an associated style sheet. Text descriptions must be made available for all image maps.
-   Client-side image maps should not be used because they cannot be properly presented to visually impaired users. If using tables for data, you must identify all row and column headers.
-   If a table has two or more rows or columns, you must use row and column headers.
-   Sites that use frames must have titles that easily enable alternative browsers to navigate through each frame. If necessary, a separate text-only site should be made available to ensure access.
-   When scripting technology is used to enable a site feature (e.g., a form), a plaintext alternative must be available that allows an assistant application to read the feature.

You can visit _https://section508.gov/content/technology-accessibility-playbook_ to read the Section 508 standards.

### World Wide Web Consortium (W3C)

This international organization creates all web standards. The following is an excerpt from [w3c.org](https://www.w3.org/):

"The World Wide Web Consortium (W3C) is an international community where [Member organizations](https://www.w3.org/Consortium/Member/List), a full-time [staff](https://www.w3.org/People/), and the public work together to develop [Web standards](https://www.w3.org/standards/). Led by Web inventor and Director [Tim Berners-Lee](https://www.w3.org/People/Berners-Lee/) and CEO [Jeffrey Jaffe](https://www.w3.org/People/Jeff/), W3C's mission is to lead the Web to its full potential. [Contact W3C](https://www.w3.org/Consortium/contact) for more information."

### Web Accessibility Initiative (WAI)

WAI aims to ensure that core technologies used on the Web, such as HTML, Cascading Style Sheets (CSS3), Extensible Markup Language (XML) and the Document Object Model (DOM), are equally accessible to all users, including those with physical, visual, hearing and cognitive disabilities. (You will learn more about these technologies later in the course.) For example, a person with a visual disability may be unable to view a multimedia presentation on the Web. One way to solve this problem is to include text equivalents of the presentation in the code. A multimedia player, such as Apple QuickTime or Microsoft Windows Media Player, could then access the text equivalent and present it to the user in Braille or as speech.

The WAI works with numerous W3C Working Groups to ensure that the standards for various W3C technologies include accessibility options. For example, the HTML standard supports improved navigation, extended descriptions of complex graphics, and multimedia captions. It also supports device-independent user interface descriptions that allow users to interact with Webpages using mouse, keyboard or voice input.

For more information, visit their website at [https://www.w3.org/WAI/](https://www.w3.org/WAI/)

Additional information about various national laws and standards is available on the W3C at [_www.w3.org/WAI/Policy_.](http://www.w3.org/WAI/Policy)

###  Web Content Accessibility Guidelines (WCAG)

Webpages should be accessible to all people, including those with disabilities. To assist in this mission, the W3C has created the Web Accessibility Initiative (WAI). The WAI has developed the Web Content Accessibility Guidelines (WCAG) to provide a universal set of standards promoting accessibility. According to the WAI, the Web's full potential can only be realized by "promoting a high degree of usability for people with disabilities." The WAI works with worldwide organizations in five main areas: technology, guidelines, tools, education and outreach, and research and development.

### W3C Authoring Tool Accessibility Guidelines (ATAG)

The W3C also addresses ways to ensure that development tools can be used by disabled people. For more information, read the W3C Authoring Tool Accessibility Guidelines at _https://[www.w3.org/TR/ATAG20/.](http://www.w3.org/TR/ATAG20/)_

ATAG focuses on two main points regarding authoring tools.

1) Make the authoring tool interface accessible

2) Support the production of accessible content

### Making Content Accessible to Users with Visual Impairment

Following are some common challenges and solutions for accommodating Web users with vision impairment:

-   **Text readability** — Make sure that fonts used are the correct size.
-   **Text support for images** — All images must be described in text using special HTML code.
-   **Screen-reader support** — Ensure that all pages and page elements can be rendered by audio screen readers.

The [Lynx](https://cects.com/using-the-lynx-web-browser/) browser is a particularly useful tool for testing web site accessibility. Lynx is entirely text based and supports braille displays and screen readers, which means that it uses the alt, name and title attributes associated with images and other non-text-based content instead of displaying the elements themselves. As such, it is a good way for testers to experience a website in the same way that a visually impaired person would.

### Making Content Accessible to Users with Audio Impairment

Following are some common challenges and solutions for accommodating Web users with hearing impairment:

-   **Alternative audio support** — If you include audio content on a page, make sure that a text-based equivalent is readily available for hearing-impaired users.
-   **Alternative speech input** —If your site includes the ability for speech input, make sure that an equivalent keyboard entry mechanism is available.
-   **Text support for audio elements** — Make sure that any audio elements are clearly marked with alternative text so that readers can obtain the information.

### Making Content Accessible to Users with Cognitive and Technical Impairments

Following are some common challenges and solutions for accommodating Web users with cognitive impairment or equipment limitations:

-   **Page content that flashes, flickers or strobes** — Such content may cause problems for those with neurological disorders.
-   **Alternative navigation** —Navigation aids should be provided to help those with lower cognitive skills.
-   **Audio support** — Audio transcriptions of text-based content may help users with reading disabilities such as dyslexia.
-   **Low-resolution alternatives** — Design Webpages so that they do not require large, expensive screen resolutions, or provide low-resolution alternatives.

## Outsourcing

Increasingly, Web development work (including site design) is being outsourced to workers in remote locations. When outsourcing occurs, a local team of workers often remains to perform some tasks (sometimes permanently, sometimes only for a short time). This local team is usually charged with managing the project. The outsourced team will probably perform the Webpage coding and other tasks that the local team cannot complete.

When working with remote teams and even other companies, you must consider the following:

-   **Non-Disclosure Agreement (NDA)** — An NDA is a legally binding contract signed by both parties stating that they will not reveal any trade secrets or intellectual property owned by the other.
-   **Legal consultation** — When signing NDAs and other documents is necessary, you should first retain legal counsel. Otherwise, you may make commitments that you cannot fulfill. Any contract breach can make your company liable for a lawsuit.

## MIME

A protocol that enables operating systems to map file name extensions to corresponding applications. Also used by applications to automatically process files downloaded from the Internet.