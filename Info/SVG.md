﻿SVG - Scalable Vector Graphics - A Graphics Markup for the Web
===============================================================

"Things to watch: SVG - Scalable Vector Graphics - at last, graphics which can be rendered optimally on all sizes of device" 
  - Tim Berners-Lee, inventor of the World Wide Web

SVG - 2d Graphics in XML
------------------------
1. SVG is a platform for two-dimensional graphics. 
   It has two parts: 
      1. an XML-based file format and 
	  2. a programming API for graphical applications. 
	Key features include shapes, text and embedded raster graphics, 
	with many different painting styles. 
	It supports scripting through languages such as ECMAScript and has 
	comprehensive support for animation.
2. SVG is used in many business areas including Web graphics, animation, user interfaces,
   graphics interchange, print and hardcopy output, mobile applications and 
   high-quality design.
3. SVG is a royalty-free vendor-neutral open standard developed under the W3C Process. 
   It has strong industry support; Authors of the SVG specification include Adobe, 
   Agfa, Apple, Canon, Corel, Ericsson, HP, IBM, Kodak, Macromedia, Microsoft, 
   Nokia, Sharp and Sun Microsystems. SVG viewers are deployed to over 100 million 
   desktops, and there is a broad range of support in many authoring tools.
4. SVG builds upon many other successful standards such as XML 
   (SVG graphics are text-based and thus easy to create), 
   JPEG and PNG for image formats, DOM for scripting and interactivity, 
   SMIL for animation and CSS for styling.
5. SVG is interoperable. The W3C release a test suite and implementation results to 
   ensure conformance.

Applications of SVG in industry
-------------------------------

Mobile

In 2001 the mobile phone industry chose SVG as the basis for its graphics platform. 
Many leading companies joined the SVG effort to produce the SVG Tiny and SVG Basic 
profiles, collectively called SVG Mobile and targetted at resource-limited devices 
such as mobile handsets and PDAs.

The SVG Mobile specification was adopted by 3GPP as the required graphics format for 
next-generation phones and multimedia messaging (MMS). 
Already there are SVG-enabled handsets shipping worldwide.
SVG Mobile is primarily used for messaging in applications such as greeting cards, 
diagrams and animations. For more details refer to the SVG Mobile specification,
authored by a subgroup of the SVG Working Group including Nokia, Ericsson and Motorola.

Print

The combination of rich graphical features, comprehensive text support and resolution 
independence in SVG produce a format suited to printing. Leading print hardware companies
are currently developing the SVG Print specification: a version of SVG specifically
suited to hard-copy output.
Use cases of SVG include an XML-based page description language similar to Postscript 
and PDF, a final-form archiving format and variable data printing, where the information 
is provided by a database and output using a graphical SVG template. SVG provides 
identical online and hardcopy display.
Being based on XML, SVG Print fits neatly into existing XML workflows. That is, 
organizations which have a data processing pipeline that supports XML can insert 
SVG Print capabilities easily into their publishing workflow, enabling dynamic document 
generation. SVG Print also integrates with common job description formats such as PODi's 
PPML and CIP4's JDF.
More details refer to the SVG Print Specification, authored by a subgroup of the SVG 
WG including Canon, HP, Adobe and Corel.

Web Applications

Web-based applications are increasing in popularity. Developers are often limited by 
browser incompatibilities and missing functionality. With powerful scripting and event 
support, SVG can be used as a platform upon which to build graphically rich applications 
and user interfaces.
With SVG, the application developer gets to use a collection of open standards. 
They are not tied to one particular implementation, vendor or authoring tool.

Design and Interchange

SVG is well suited to the high-end graphical design market common in the Aerospace, 
Transportation, Automotive and Telecommunication industries. The extensibility of XML 
allows SVG diagrams to have embedded metadata in proprietary formats without affecting 
the presentation.
For example, a CAD program could export to SVG for online display, but embed data within 
the file that facilitates future editing or roundtripping.
Also, since many design tools support import and export of SVG, it can be used as an 
interchange format between applications.

GIS and Mapping

Geographic Information Systems have very specific requirements: rich graphics features, 
support for vector and raster content and the ability to handle a very large amount 
of data. SVG is well-suited to this market and many GIS systems provide SVG export.
Like the design case mentioned above, the ability to extend SVG and embed metadata is 
useful to the mapping community. For example, graphical elements can be identified as 
their native objects (such as a lake), allowing applications to interact with the 
objects in a graphical manner.
SVG is a perfect complement to the OpenGIS consortium's GML format. GML, also XML-based, 
describes geographical elements such as rivers and roads. It can be converted into SVG
using an XML pipeline for online display.

Embedded Systems

Most embedded systems have severe resource limitations, including smaller screens, 
limited memory and reduced processing capability compared to typical desktop systems. 
The SVG Mobile specification was designed for such devices and allows for the 
development of graphical user interfaces for embedded systems. In its support for 
input events and scripting, devices can use an SVG frontend for control and 
monitoring, such as a control system for industrial devices.

Technical Details

SVG is a language for describing two-dimensional graphics in XML. SVG allows for three types of graphic objects: vector graphic shapes (e.g., paths consisting of straight lines and curves), images and text. Graphical objects can be grouped, styled, transformed and composited into previously rendered objects. Text can be in any XML namespace suitable to the application, which enhances searchability and accessibility of the SVG graphics. The feature set includes nested transformations, clipping paths, alpha masks, filter effects, template objects and extensibility.
SVG drawings can be dynamic and interactive. The Document Object Model (DOM) for SVG, which includes the full XML DOM, allows for straightforward and efficient vector graphics animation via scripting. A rich set of event handlers such as onmouseover and onclick can be assigned to any SVG graphical object. Because of its compatibility and leveraging of other Web standards, features like scripting can be done on SVG elements and other XML elements from different namespaces simultaneously within the same Web page.


SVG
====
Scalable Vector Graphics (SVG) is a Web graphics language. 
SVG defines markup and APIs for creating static or dynamic images, capable of 
interactivity and animation, including various graphical effects. 
It can be styled with CSS, and combined with HTML. This document provides an 
introduction to SVG, with examples and explanations.

SVG or Scalable Vector Graphics is a relatively new World Wide Web Consortium (W3C) 
standard, used by a host of companies and organizations, for the creation and display 
of vector graphic material. SVG is an XML language that allows dynamic creation of 
content using JavaScript within or outside the context of the World Wide Web.

Advantages of SVG
==================
SVG has some advantages over conventional bitmapped graphics, such as JPEG, GIF, and PNG, 
used in the browser environment, because of several reasons:

1. The files are generally much smaller than bitmaps, resulting in quicker download times.
2. The graphics can be scaled to fit different display devices without the pixelation 
   associated with enlarging bitmaps.
3. The graphics are constructed within the browser, reducing the server load and network 
   response time generally associated with web imagery. That is, a typically small 
   formulaic description is sent from the server to the client. 
   The client then reconstructs the imagery based on the formulas it receives.
4. The end-user can interact with and change the graphics without need for complex and 
   costly client-server communications.
5. It provides native support for SMIL (Synchronized Media Integration Language) meaning 
   that animations, for example, are supported with a more analog notion of timing, 
   hence freeing the programmer from timed loops typically used in JavaScript-based 
   animations.
6. It responds to JavaScript: the same scripting language used in the HTML environment. 
   This means the two types of documents may converse, share information and modify one 
   another.
SVG is an XML language. This is important for at least three reasons. First, the 
code tends to adhere to agreed upon standards of how SVG should be written and how 
client software should respond. Second, like all XML, it is written in text, and 
can generally be read not only by machines but also by humans. Third, and perhaps 
most importantly, JavaScript can be used to manipulate both the objects and the 
Document Object Model, in ways quite similar to how JavaScript is used in conjunction 
with HTML. If you already know how to use JavaScript and HTML for web-programming, 
the learning curve will be pretty gentle, particularly in view of the benefits to be 
gained.

