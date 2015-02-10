---
layout: page
title:  "HTML &amp; CSS Basics"
name: "Week 4"
description: "Picking up where the Web Skills class left off, we'll review HTML tags, nesting, and attributes. We'll also review basic CSS selectors and properties."
date: 2015-02-16
next: week5
previous: week3
type: lesson
readings: [
    {
        "title" : "Chapters 10 - 12: HTML & CSS"
    }
]
downloads: 
quizzes: 
assignment: 
---

Make sure you have all the required software installed before this class, as we'll double check your settings and development environment. We'll also learn to snoop our sites with Chrome's Inspector.

=======
<h5>News Package Critique</h5>
<ul>
    <li>Group 1: Sasha L, Mara V.</li>
    <li>Group 2: Gina P, Philippe J.</li>
</ul>

###Review of HTML 

In this section, we will do a review of HTML we learned in Web Skills. 

###HTML Tags

<img src="/assets/images/html-tags.jpg" class="img-responsive left-block" alt="HTML tags" />

Remember that most HTML tags have two parts:

* Opening Tag <code>&lt;p&gt;</code>
* Closing Tag <code>&lt;/p&gt;</code>

The closing tag has a forward-slash before the end of the name.

###Attributes

It's important that we understand **attributes** which are pieces of information that can go into tags.

<img src="/assets/images/attribute.jpg" class="img-responsive left-block" alt="An attribute in a single tag" />

Attributes like `href=""` go inside the &lt;a&gt; tag to specify where a user will go when they click a link.

####Some commong attributes

* **src** — Specify the image location inside a &lt;img /&gt; tag.
* **alt** — Specify some alternate text to describe the image in an &lt;img /&gt; tag.
* **href** — Specify the URL an &lt;a&gt; tag will visit when clicked.
* **title** — Specify some text that will appear when the user hovers their mouse over this tag.

####Attributes to use for CSS

There are three attributes that can go in all HTML tags that pertains to CSS:

* **id** attibute — This is a unique term that gives this tag an identifier we can reference in our CSS.
* **class** attribute — This is a grouping term that allows us to reference multiple tags in our CSS.
* **style** attribute — This is a special way to include *inline* CSS, basically putting CSS code directly into an HTML tag.

####Boolean Attributes

Later, when we get into video, you may see some attributes with no value assigned. These are boolean attributes, which means they either exist or they don't, which determines whether they are true or false. If they are present, it is assumed they are true. One common place these are seen is in the &lt;video&gt; tag. You can optionally include player controls, or remove the attribute altogether, to have a chromeless video play.

<img src="/assets/images/attribute-with-no-value.jpg" class="img-responsive left-block" alt="attributes with no value" />

In the above example, the **preload**, **controls** and **loop** attributes do not assign a value (there is no equals symbol). If they are present, then they set those properties of the video.


###Data Attribute

The **data** attribute will be important later when we do JavaScript. This attribute allows us to include some arbitrary data to HTML tags, which can be used by plugins or many other JavaScript utilities.

Data attributes always start with the word **data** and then end with a hyphen. The words that come after that depend on the plugin being used. There might be a plugin that wants the word "slideshow" as a data attribute. In your html tag, you might include: `data-slideshow="true"` The data keyword here is slideshow, and the value you assign it is true. 

In this example below, a plugin called Cycle has some properties you can assign:

<img src="/assets/images/attributes-data.jpg" class="img-responsive left-block" alt="data attributes" />


###Video and Audio Tags

There are some relatively new special HTML5 video tags that allow you to display video files right in the browser without any special players or other code. 

```html
<video width="800" height="600" poster="image.jpg" preload controls loop>
	<source src="path/to/video.mp4" type="video/mp4" />
	<source src="path/to/video.webm" type="video/webm" />
	<img src="fallback.jpg" />
</video>
```

The video tags takes the following attributes:

* **preload** — The browser should preload the video so it's ready to play at a moment's notice.
* **src** — Set the URL of the video file
* **poster** — An image people will see before your video plays.
* **controls** — Controls like a stop/play/mute button, and a scrubber along the bottom where people can skip ahead.

The two &lt;source&gt; tags offer two more more options for video files to be loaded. This creates a fallback system in case the browser doesn't support a particular video type. (Firefox doesn't support H.264 mp4 files, for example.) We will use a conversion software to convert from mp4 to webm, which is supported by Internet Explorer and Firefox.

**Note: Please see Page 214 in HTML &amp; CSS book for more information.**

###Relative vs Absolute Paths

A path is the location of files that pertain to your web page. We often list paths in attributes like `href=""` or `src=""`. How you write your path, particularly the characters you use to start the path, determine where the browser will look for the files.

Paths take the following forms:

* **URL paths** — These are paths that use a protocol to retrieve content out on the web, perhaps another server.
* **Relative paths** — These are paths that start from the current file's location, and you either work your way up or down the document tree.
* **Absolute paths** — These are paths that always start from the root folder of a website, regardless of where your file is.

<img src="/assets/images/folder-structure.jpg" class="img-responsive left-block" alt="folder structure" />

####URL Paths

These start with a protocol, like `http:` or `https:`. These will go out onto the web and fetch a web page somewhere based on the URL given. Everything after that is an absolute path.

**Note: Please see Page 81–84 in HTML &amp; CSS book for more information.**

