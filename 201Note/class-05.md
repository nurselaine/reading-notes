# Class 05 Reading Notes

<hr>

## Chapter 5: “Images” (pp.94-125)
- Create an images folder in each project to stay organized
- **img tag** 
  - src: tells browser where to find image
  - alt: provides text of image , always add alt even if value is empty for stock
  - title: also provide text of image/extra info (alttext)
- Placement
  - before paragraph: block elements
  - inside start of paragraph: inline elements
  - in middle of paragraph: inline elements, if img element is inside block element, any text or inline elements will flow around images
- align: old HTML to control flow of imgs ; best practice to use CSS
- Rules (3) 
  1. saves images in correct format: jpeg, gif, png or else poorer quality
    - JPEG is good for coloful images
    - GIF/PNG for images with few color/large areas of same color
  2. save images at right size to avoid distortion 
  3. correct resolution: larger resolution = larger image 
- Adobe photoshop to edit 
- Dimensions: save width and height you want them to appear
  - check size of img by right clicking 
- figure element used to contain img with caption
## Chapter 11: “Color” (pp.246-263)
- RGB red green blue (000, 000, 000, [opacity]) 0-255
  - opacity: 0.0-1.0 more transparent to opaque
- hex codes six digit codes preceded by a #000000
- Color names: 147 different colors
- HSLA: hue saturation lightness alpha
  - alpha: 0-1.0 represents transparency
- hue: 
- saturation: amount of gray in color
- brightness: amount of black in color
- contrast: in context of whether text is legible
  - low, high, medium (harder to read the lower the contrast)

## Chapter 12: “Text” (pp.264-299)
- Serif: extra details on the end
- sans-serif: straiht ends
- mono space: every letter is the same width
- cursive: handwriting styles, joining stroke
- fantasy: decorative fonts used for titles
- anatomy of text:  
  - Ascender: cap height, top of flat letters
  - X-height: height of the letter x
  - baseline: line all letters lie on
  - decscender: below the baseline
- weight: light, medium, bold, black
- style: normal, italic, oblique
- stretch: bondensed, regular, extended
- font size: px, %, ems | default size 16px | **use px for best practice**
  - % 200% = 32px
  - 1 em = width of letter m | change size of text relative to size of text in parent element
  - pleasant scale for text: 8, 9, 10, 11, 12, 14,18,24,36,48,60,72
- text-transform: like javascrip toupper/lowercase method
- text-decoration: blink, animates text to make it flash!
- leading: certical space between lines of text, line-height property sets height for entire line of text
- Kerning: space between each letter, word-spacing property: **ems value**


<hr>

## JPEG vs PNG vs GIF
- use JPEG format for all natural scenes for better color
- PNG is good for img that needs transparency or object with sharp contract
- gif for animations
- compression: lossless & lossy, information loss
  - JPEG lossy compression
  - PNG lossless, no data lost during compression - higher quality & sharper
  - GIF lossless 
- Transparency: something completely invisible
  - JPEG doesn't support transparency
  - PNG: inserts alpha channel or declares transparency as color
  - gif supports by declaring transparency as color
- Colors
  - JPEG: supports 16 million colors
  - PNG: types PNG8 supports 256 and PNG8 support 16 million colors
  - GIF supports 256 colors
NOTE: The post has a TL;DR you might find handy.

## Things I want to know
- I want to know how to position multiple pictures on top of each other and to organize in a way that is aesthetic on a webpage
- I want to find my go to fonts that are simple and basic
- I would like to learn how to pick the most suitable stock photos for web pages without taking so long to find the right one
