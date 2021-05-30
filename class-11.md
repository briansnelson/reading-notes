# Class 11 Readings: Audio, Video, Images

## Duckett Chapter 16 "Images (406-427)

### Summary of Chapter 16

- You can specify the dimensions fo images using CSS. Helpful when you use the same sized images on several pages.
- Images can be aligned horizontally and vertically
- can use a background image behind the box created by any element on a page.
- background images can appear just once or be repeated across the background of the box
- you can create images rollover effects by moving the background position of an image.
- Use sprites to reduce the number of images browser must load

## Duckett Chapter 19 "Practical Information"

### Summary of Chapter 19

- SEO helps visitors find your sites when using search engines
- Analytics tools such as Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there
- To put your site on the web, need a domain name and web hosting
- FTP programs allow you to transfer files from local computer to web server
- Many companies provide platforms for blogging, email, newsletters, e-commerce and other popular website tools

## MDN article: Video and Audio APIs

This article is about how to imbed video and audio APIs into HTML5. Video and Audio elements allow this capacity. 
Example: 
`<video controls>
  <source src= "rabbit320.mp4" type="video/mpr">
  <source src="rabbit320.webm" type="video/webm">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4"> link to the video</a>
  </video>`

There is a zip file to download: HTMLMediaElement. This article tells you how to use the HTML, CSS, and JS. 

### Summary of article:

HTMLMediaElemnt API makes a wealth of functionality available for creating simple video and audio players. 
This is only the beginning. 

- Suggestions to enhance existing example:

1. The time display currently breaks if the video is an hour long or more (well, it won't display hours; just minutes and seconds). Can you figure out how to change the example to make it display hours?

2. Because <audio> elements have the same HTMLMediaElement functionality available to them, you could easily get this player to work for an <audio> element too. Try doing so.

3. Can you work out a way to turn the timer inner <div> element into a true seek bar/scrobbler — i.e., when you click somewhere on the bar, it jumps to that relative position in the video playback? As a hint, you can find out the X and Y values of the element's left/right and top/bottom sides via the getBoundingClientRect() method, and you can find the coordinates of a mouse click via the event object of the click event, called on the Document object. For example:






