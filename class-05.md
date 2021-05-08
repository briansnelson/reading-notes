# Reading Notes Day 5: HTML Images; CSS Color & Text

## Duckett's HTML Book: Chapter 5, 11, 12 and blog post by Rahul Nanwani JPEG vs PNG vs GIF

## HTML Images, Chapter 5

# 4 learning points in this chapter

1. Include an image in webpage using HTML
2. Pick which image format to use
3. Show an image at the right size
4. Optimize an image for use on the web to make pages load faster -- my guess here is less is more.

# This book only shows the stock image sites that one must pay, not the public domain images. Too bad

# How to add an image:
Use the `<img>` element, which is not a tag becasue there is no closing tag. The following elemenst sit inside the `>`. `src` means source, and tells the browser where to find the image; `alt` provides the text description for blind people, and the `title` attribute can provide additional information about the image. Most browsers will display this content in a tooltip when the user hovers over the image. 
EXAMPLE: `<img src="images/grit360.jpg" alt="Logo for Grit360" title="GRIT360 we build, we connect, we create, we inspire" />

# Height & Width of images: uses pixels.

EXAMPLE: `<img src="images/grit360.jpg" alt="Logo for GRIT360" width="600" height="450" />



## Blog Post: JPEG vs PNG vs GIF

# JPEG, PNG and GIF comprise 95% of all images on the web

# Use Hueristic

- JPEG for natural scene of photgraph with variation in color and intensity is smooth.
- PNG for transparency or images with text & objects with sharp contrast edges like logos.
- GIF for any animation

# Compression comes in 2 types

- lossless
- lossy


