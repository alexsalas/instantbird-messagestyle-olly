Olly.js (1.0)
=======

A JavaScript library to convert URLs into embedable HTML.

Example
-------

[Live Demo](http://abeisgreat.github.io/Olly.js/markup/example.html)

Usage
-----
After being included with a `<script>` tag, Olly exposes the `olly` object (weird, right?). This object has one important method `olly.embed`. This method takes, at a minimum, a URL from a supported service and a DOM element. The method then fills the provided element with the rich media from the provided URL. For example, a link to a Youtube video will fill the provided element with an embedded Youtube player for the video:

    olly.embed("https://www.youtube.com/watch?v=x-8QAFqAAJ8", document.getElementById("youtube"));
    
This will fill `#youtube` with the following markup.

    '<embed width="420" height="345" src="http://www.youtube.com/v/x-8QAFqAAJ8" type="application/x-shockwave-flash">'
    
Supported Services
------------------

**Video**

* Youtube
* Vimeo
* Twitch.TV

**Audio**

* Soundcloud

**Images**

* Imgur
* Gfycat

**Social**

* Reddit Subreddits and Users
* Twitter Tweets

**Other**

* Github Repos
* jsFiddle

Supported File Types
------------------

**Video**

* MP4
* WebM
* OGV

**Images**

* JPG
* PNG
* BMP
* GIF

**Audio**

* MP3
* OGG

*... and any other you want to implement, pull requests are appreciated!*