---
layout: page
title:  "Adding Interactivity"
name: "Week 10"
description: "We'll introduce JavaScript and jQuery in order to add interactivity to our story designs. We will learn the basics of hiding, revealings and modify our content dynamically. And we'll discuss how this can enhance our story experience."
date: 2015-04-06
next: week11
previous: week9
type: lesson
readings: [
    {
        "title": "Code School jQuery Tutorial",
        "url": "http://try.jquery.com/"
    },
    {
        "title": "Code Academy jQuery Tutorial",
        "url": "http://www.codecademy.com/tracks/jquery"
    }
]
downloads: [
    {
        "title": "Class exercise file and homework",
        "url": "../assets/zip/jquery.zip"
    },
    {
        "title": "PDF of the presetnation given in class",
        "url": "../assets/pdfs/jquery.pdf"
    }
]
quizzes: 
assignment: 
---

<h5>News Package Critique</h5>
<ul>
    <li>Group 1: Alicia V, Justin W.</li>
    <li>Group 2: Leah W, Melissa B.</li>
</ul>


###jQuery Cheat Sheet

####To make jQuery availabile in your document

1. Add jQuery script tag to your document, typically right before the closing &lt;body&gt; tag.

```html
<script src="http://code.jquery.com/jquery-latest.js"></script>
```

2. Add a script tag and insert the jQuery "ready" function.

```html
<script>
jQuery(document).ready(function($){

    //code goes here

});
</script>
```

####Parts of a jQuery statement

<img src="{{ site.baseurl }}/assets/images/tutorial-jquery.png" class="img-responsive left-block" alt="jQuery statement" />


####Anatomy of a function

<img src="{{ site.baseurl }}/assets/images/tutorial-jquery-function.png" class="img-responsive left-block" alt="jQuery function" />


####Example of click in action

When using click or hover, always place the action code within the curly brackets. To make the code more readable, separate the brackets on new lines, and use indentation. 

Make an element disappear when clicked - The following command will make an HTML element with id="closeDiv" disappear when a button is clicked.

```javascript
$("#button").on("click", function(){

    $("#closeDiv").hide();

});
```

####A list of common jQuery methods

```javascript

$("#mybox").hide();                 //make an element disappear instantly 
$("#mybox").show();                 //make an element appear instantly 
$("#mybox").fadeOut(400);           //make an element fade out
$("#mybox").fadeIn(400);            //fade in an element that is already invisible
$("#mybox").fadeTo(400, 0.8);       //fade to specific level of transparency
$("#mybox").fadeToggle(400);        //will fade in or out
$("#mybox").slideDown(400);         //slide an element down to display
$("#mybox").slideUp(400);           //slide an element up to display
$("#mybox").slideToggle(400);       //slide depending on current state
$("#mybox").css("color", "black");  //change the css of an element
$("#mybox").html('<h1>hi</h1>');    //change the HTML of an element (use single quotes)
$("#mybox").attr("src", "pic.jpg"); //add an attribute to an element
$("#mybox").text("hello");          //add text to an element


$("#mybox").on("click", function(){
    //do something on click
});       

$("#mybox").on("dblclick", function(){
    //do something when double-clicked
});         

/* Other mouse events that can be used with "on" method include:

click
dblclick
contextmenu (right-button mouse click)
mouseout
mousemove
mouseover
mouseup
mousedown

*/
```




