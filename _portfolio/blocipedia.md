---
layout: post
title: BlocJams
thumbnail-path: "img/bloc_jams_bg.jpg"
short-description: BlocJams is a spotify replica for playing some great classical music.

---

{:.center}
![]({{ site.baseurl }}/img/bloc_jams_bg.jpg)
<a href ="http://pirate-duck-24278.netlify.com/">Link to BlocJams </a>

## Explanation

Bloc Jams is a limited replica of Spotify. The emphasis of this project is CSS and DOM manipulation.  The music player is controlled by custom jQuery scripts. The exception being that I use a library to actually handle the playing of the audio files. Check it out and listen to some classic tunes!

## Problem
There is a property on the window object called onload that we can pass a function that executes when the window (like a browser window or tab) finishes loading. I added the window.onload property to landing.js and pass it an anonymous function that calls a JavaScript alert():

## Solution

We assign the window.onload property an event handler, a function that handles code in response to an event. The event handler executes as soon as an action fires an event.

As a page loads, the browser may render elements, styles, and scripts that require additional time to process. This means that some DOM nodes may not exist until the browser finishes loading the page. Put any code that is dependent on a completely-loaded web page in a window.onload block, particularly any code that depends on DOM elements to execute properly


## Results

The bloc-jams site uses Bootstrap Angular to create a serve that controls song playback. Using JQuery was a great tool but learning to build a more sophisticated front end application using Angular was very productive. Learning Angular will be a very useful tool for future projects
