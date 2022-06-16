This article covers the following items:

-   <video> element
-   Video formats
-   <audio> element
-   Audio formats
-   Image maps
-   Image transparency
-   Image interlacing
-   Animation

## The <video> element

The <video> element was introduced with HTML5 and is used to add video to a webpage. Below is an example of the <video> element:

<video controls>

<source src="video.mp4" type="video/mp4">

<source src="video.webm" type="video/webm">

<source src="video.ogg" type="video/ogg">

Your browser does not support the HTML5 video element.

</video>

**Item**

**Description**

<video>

HTML5 element used to insert video onto a webpage

<source>

Element used to specify a media resource

controls

Attribute that allows the user to play, pause, and adjust audio settings

src

Attribute used within the <source> tag to specify the media file

type

Attribute used within the <source> tag to specify the type of video (mp4, webm, ogg)

Visit W3Schools to [practice using the <video> element](https://www.w3schools.com/html/html5_video.asp). What other attributes can you include within the <video> tag?

### Video file formats

**The <video> element supports three file formats: MP4, WebM, and Ogg.**

Modern major browsers support these file formats, except Safari. Safari does not support Ogg.

The MP4 video format (MPEG 4 files) is widely used. Popular video sites such as YouTube have every video available in the MP4 video format. MP4 often uses the H.264 video codec, which is native to most browsers that support HTML5. This codec uses far less processor and battery power because it does not require a plug-in.

H.265 is a potential successor to the H.264 codec. It can potentially offer almost double the data compression of H.264 without any loss to video quality. It also supports up to 8K resolutions (8192×4320). Although 4K video is not a standard that is widely used, H.265 is positioned to be the codec of choice should that change. A great deal of systems do not support the H.265 codec, so it is advisable that any content deployed using it also be offered with more conventional codecs. The WebM and Ogg video formats are also used. The WebM video format often uses the VP8 codec. VP8 is an open video compression format owned by Google. Ogg uses the Theora format for HTML5 video, which is a free video compression format that can be distributed without licensing fees.

WebM is a free, open-source alternative to the MP4 video format. It uses the .WEBM file name extension and is part of the Alliance for Open Media. Their development is sponsored by Google. The WebM format uses separate codecs for audio and video encoding. WebM uses VP9 as its video coding format and opus as its audio coding format. Both of these coding formats effectively compete with, and sometimes outperform their proprietary competition. This makes WebM a widely used, efficient video file format. YouTube, the world's largest video site, encodes all of its videos into WebMs due to the format's efficiency and quality.

To ensure all browsers and devices can access your video, you should format your video to these three formats and identify them in the <source> element. If that is not possible, then choose one, such as the MP4 format, as the default format.

## The <audio> element

The <audio> element was introduced with HTML5 and is used to add audio to a webpage. Below is an example of the <audio> element:

<audio controls>

<source src="audio.mp3" type="audio/mp3">

<source src="audio.wav" type="audio/wav">

<source src="audio.ogg" type="audio/ogg">

Your browser does not support the HTML5 audio element.

</audio>

<audio>

HTML5 element used to insert audio onto a webpage

<source>

Element used to specify a media resource

controls

Attribute that allows the user to play, pause, and adjust audio settings

src

Attribute used within the <source> tag to specify the media file

type

Attribute used within the <source> tag to specify the type of audio (mp3, wav, ogg)

Visit W3Schools to [practice using the <audio> element](https://www.w3schools.com/html/html5_audio.asp). What other attributes can you include within the <audio> tag?

### Audio File Formats

**The <audio> element supports three file formats: MP3, WAV, and Ogg.**

Modern major browsers support these file formats, except Safari. Safari does not support Ogg.

## The <iframe> Element

**The <iframe> element is used to embed a document hosted on another domain**, such as YouTube or Google Maps. An iframe is displays a web page within a web page.

Examples:

               **YouTube**:

<iframe width="560" height="315" src="https://www.youtube.com/embed/UB1O30fR-EE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Google Maps**:

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3025.502337165393!2d-111.87213558428806!3d40.68493304720729!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x87528a6e0a6f5605%3A0  
x6387fef1611b1ea2!2sWestern%20Governors%20University!5e0!3m2!1sen!2sus!4v1632752017761!5m2!1sen!2sus" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>

**w3Schools**:

<iframe src="https://www.w3schools.com" height="500" width="800" title="Iframe Example"></iframe>

The width and height attributes specify, in pixels, the size of the <iframe> element. The _src_ attribute is the address for the document you are looking to embed. Enclosing text between the <iframe> tags is a best practice, as this text will display in any browsers that do not support it. This should be infrequent, however, since all major browsers support the <iframe> element.

Visit W3Schools to [practice using the <iframe> element](https://www.w3schools.com/html/html_iframe.asp).

## Graphics

Two types of graphical images are used within Webpages:

1.  **Vector** — graphics that use mathematical coordinates with lines, curves, and shapes to create images and specify colors. Vector graphics can be created using various software tools, such as Adobe Illustrator. Vector graphics are generally small in file size. Vector graphics are scalable, which means they keep their image quality when enlarged or shrunk.
2.  **Bitmap** — graphics that use small dots (usually thousands) to create images and specify colors. Each dot is mapped to bits stored in a computer's memory. Bitmaps are also called raster graphics, and they include the JPEG, GIF and PNG formats. Digitized photographs are the most common type of bitmap seen on the Web. Bitmap images can be created using software tools such as Microsoft Paint. Making bitmap images more detailed can create large file sizes. Removing pixels and compressing files will decrease file size but will also reduce image quality.

### Image Transparency

An image that supports transparency provides the visual effect of blending into the background of your Webpage. When used, the page background simply shows through the transparent part of the image file. Most developers use image transparency to remove the blank image background, so it appears to float on the page. However, you can make any element of an image transparent, not just its background.

**The only Web-ready image file formats that support transparency are GIF, PNG and SVG. The JPEG, BMP and TIFF formats do not support transparency on the Web.**

Here is an [example of an image with and without transparency](https://looka.com/blog/transparent-logo/).

### Image Interlacing

Interlacing is a technique that allows an image to progressively display in a browser as it downloads. The image will appear in stages over the period of downloading time. This action makes your pages more accessible to users with slower Internet connections. This was important during the days of dial-up, but not widely seen with today’s broadband Internet connections.

Standard image formats are read from top to bottom. The top of a non-interlaced image will appear after the browser has read 50 percent of the image. The bottom half will render sometime later.

By contrast, an interlaced image appears to fade in as it renders in the browser because it is interpreted differently. An interlaced image is repeatedly scanned from left to right**. The first pass will render roughly 13 percent of the entire image. The second pass delivers 25 percent, and then continues in 25-percent increments until the image renders completely. During this process, the full image will at first appear fuzzy, but will continuously sharpen.**

The only **Web-ready image file formats that support interlacing are GIF and PNG**. Both GIF formats, 87a and 89a, support interlacing. You can create an interlaced image by configuring an image file in a graphics-editing application and saving it as a compatible file type.

### Animation

The only Web-ready image file formats that support animation are GIF, PNG and MNG. Programs such as the Alchemy Mindworks GIF Construction Set allow you to incorporate several images into one file.

Flash Animation was once widely used in websites. Flash was created by Adobe and used macros to manipulate vector-based graphics to create animation. It was a type of proprietary software. Support for Flash ended December 2020.

### Scalable Vector Graphcs (SVG)

Scalable Vector Graphics (SVG) is a W3C-recommended language developed by various vendors, including Adobe, Microsoft and Sun. SVG uses XML to describe graphics and graphical applications. SVG allows you to create cross-platform animated movies. Not all SVG images are animated, but this application is common because SVG offers comprehensive animation support. Unlike Flash, SVG is an open standard. However, it provides similar features in addition to animation, including:

-   **Compression** — The compression algorithms available in SVG allow you to create high-quality images and movies that are smaller in file size than other formats. SVG images have more efficient compression than JPG or GIF images.
-   **Searchable text** — Text within SVG images can be indexed and searched.
-   **Zooming** — You can zoom in on portions of an image without losing image quality. SVG supports other technologies, including JPEG, GIF and Java. As with Flash, a browser must be updated with a plug-in to render SVG data, but all major vendors incorporate support for SVG. To learn more about SVG, visit _[www.w3.org/Graphics/SVG](http://www.w3.org/Graphics/SVG)_.

Check out [snapsvg.io/demos](http://snapsvg.io/demos/) for some great examples of SVG and JavaScript in action.

### Image Layers

When you design an image, each individual component of the image can be created on its own layer, thus allowing that component to be manipulated independently of the entire image. A series of layers will compose an entire image, and an image can have as many layers as necessary.

However, although layers are supported in the PNG file format, they are not supported by GIF or JPG formats. This means that when the image is finalized, it must be flattened into a single layer to be exported to those formats, and then the layers can no longer be manipulated. If you maintain a copy of the original layered version of the image, you can make changes easily, and other versions of the image can be exported when necessary.

## Image Map (Hot Spot)

An image map is an image that includes hyperlinks within specific areas of the image. These linked areas, or hot spots, are defined by a set of coordinates.

The following tags are used to create a hot spot: <img>, <map>, and <area>. See example below.

<img src="imagemap.gif" usemap="#mapname">

<map name="mapname">

<area shape="shape" coords="coordinates" href="url" alt="description">

<area shape="shape" coords="coordinates" href="url" alt="description">

<area shape="shape" coords="coordinates" href="url" alt="description">

</map>

Visit W3schools.com for an example and to [practice creating an image map](https://www.w3schools.com/html/html_images_imagemap.asp).

### Possible hot spot shapes

-   **rect**: used to create a rectangular area
-   **circle**: used to create a circular area
-   **poly**: used to create a polygonal area
-   **default**: used to define the entire area