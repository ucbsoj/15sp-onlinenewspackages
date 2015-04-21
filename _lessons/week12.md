---
layout: page
title:  "Applied Interactivity"
name: "Week 12"
description: "We'll cover some freely available 3rd-party tools - like PopcornMaker, TimelineJS and SoundCiteJS - for adding interactivity to our projects."
date: 2015-04-20
next: week13
previous: week11
type: lesson
readings: 
downloads: 
quizzes: 
assignment: 
---

<h5>News Package Critique</h5>
<ul>
    <li>Group 1: Alissa G, Elina S.</li>
    <li>Group 2: Theodore A, Lakshmi E.</li>
</ul>

##jQuery Examples

You can download the [jQuery examples file here.](https://github.com/ucbsoj/jquery-examples/archive/gh-pages.zip)

This file is also hosted on the web here: [http://ucbsoj.github.io/jquery-examples/](http://ucbsoj.github.io/jquery-examples/)

The [presentation given in class (PDF)]({{ site.baseurl }}/assets/pdfs/jquery-plugins.pdf).

###Premiere Export Settings

Use these settings if you plan to export your video for uploading to **Vimeo or YouTube**.

* **Format:** H.264  
* **Preset:** Vimeo/YouTube 1080p HD  
(all other settings will be done automatically based on the preset you pick)

Use these settings if you plan to export your video to embed directly in the HTML5 video tag (i.e. background video on the page).

* **Format:** H.264  
* **Preset:** Custom  
* **Export Video/Export Audio:** Check only what you need  
* **Width/Height:** Background video should generally be less than 700px wide  
* **Framerate:** Match the source, which should display in the summary section  
* **Field Order/Aspect/TV Standard:** Based on Source  
* **Profile/Level:**  
	* Baseline 3.1 (to support older iPod/iPhone 3G)  
	* Main Level: 3.1 to support only iPhone 4 and above. [Info](https://developer.apple.com/library/ios/documentation/NetworkingInternet/Conceptual/StreamingMediaGuide/FrequentlyAskedQuestions/FrequentlyAskedQuestions.html))  
* **Render at Maximum Depth:** Checked  
* **Bitrate Encoding:** VBR, 2 pass (1 pass if you're in a hurry)  
* **Target/Maximum Bitrate [Mbps]:**  
	* Less than 1 mbps (low to medium quality, good for background video)
	* 1–3 mbps (higher quality)
	* 3+ mbps (very high quality)

The goal with setting the bitrate is to encode your video at an acceptable quality while keeping the filesize as small as possible. This only pertains to HTML5 video. If you're uploading to Vimeo or YouTube, you generally want an even higher quality because they will further downsample the video when you upload to their servers.


