# Css is thinking 'inside the box' 

## CSS means Cascading Style sheets 
-html is the language for the structure and content of the website, CSS is the language for design. 
-It modifies the information (color, font, size) inside of the HTML.
-External vs Internal-better to separate (external) if webpage is larger than one page.

## Color
-Rgb
    * red, blue, green
color: RGB= Red/Green/Blue.
Hex codes represent values for red, green, blue in hexadecimal code.
147 color names
Hue:
Saturation is how much gray .
Brightness: How much black is in color
Contrast: Text is easeir to read in high contrast, but can get tiring if long passages.
Opacity opacity rgba: is set between 0.0-1.0
CSS3; HSL Colors: Hue, Saturation, Lightnes

So--it seems there are a few different 'dials' to make color.
Color name, hex Codes, RGB values. Then there are finer aspects of the color itself.
another way to think of it is big rocks and smaller definitions of those rocks.

Review with Brad: CSS means Cascading Style sheets
reads top to bottom
Specificity by selector  - types, classes, id, universal !important `<p>`, {curly bracket}
Types: h1, h2, span, div, header
  example: h1 {this means for all h1 types}
class -
rule set  
h1 {color: blue; // declaration property/value
    background-color: pink;}
  `<h1 id="firsth1">`color me blue</>
  
  group things like this: p, img, header {make rule set} that applies to all
  
  Linking:
  `<head>`
   >link rel="stylesheet" href="myCssFile.css">
   command ? makes everything comment the line.
   header
   `<nav`
