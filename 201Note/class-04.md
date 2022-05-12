## Chapter 4: Ch.4 “Links” 
- anatomy of link 
  - < a > element
  - href: hold link of page 
  - link text: user can add text between 
  - attributes:
    - target:_blank to open link in new window
    - id can be given to specify places on a page to later be used to help create nav bar for user to select where on page to go
      - href="#id-location"
      - same syntax applies for linking specific part of another page
- ## images
  - use an images folder/ interface folder for logos and buttons
  - img tag
    - src attribute: provide relative ural
    - alt: text description of img
    - title: additional info about img
<hr>
  opening & closing text
    - absolute url: full web address for page
      - domain name for site
      - path to specific page or homepage
    - relative url: other pages within same site, use shorthand
      - change path to file name for specified page
      - use foward slash to specify which folder to link | specify with name of folder or ../ as parent 
      - **/** will return homepage
- Email Links:
  - use a tags
  - set href="mailto:email@gmail.com", mailto keyword

- URL: uniform Resource Locator, unique to each 
web page
- Organize code by places pages for different sections in different folders
  - root: contains all files
<hr>

## Chapter 15: “Layout” 
- Div: groups multiple block level elements together
- Positioning scheme:
  - **Normal flow**: block elements appear below each item
    - position: Static, 
  - **relative**: shifts elements to top, right, bottom, or left
    - define top, left, right, or bottom to move element 
  - **absolute**: position relative to containing element; ignores surrounding elements and moves with users scrolling
    - fixed positioning: position in relation to browser to make item stay in position when scrolling 
- **box offset**: 
  - fixed: position in relation to browser window, don't effect surrond elememt
  - **floting**: floating element takes element out of normal flow and position Left and right - is a block level element
    - indicate width propery to keep results consistent
    - if containing elements only contain floated element, height maybe default 0px
      = Solution: clear property, overflow: auto
  - use Z index: controls which box overlaps/ stacking content
  - multi-colum layouts
    - width: sets width of columns
    - float: positions columns next to each other
    - margin: creates gap between columns
    - Screen sizes
    - resolution: number of dots a screen shows per inch - high resolution, smaller text appears
      - 960-1000 pixels when creating pages
- Liquid Layouts: stretch and contract as user screen increases/decreases (uses percentages)
  - Use min-width and max-width to create boundaries 
- fixed width layout: specify width of mian boxes on page
  - rule: body element is used to fix the width of page at 960px and cemtered via margin: auto
  - rule: set width to 90% to leave samll gap between browser sides
- CSS frameworks: s creating layout grids, styling forms, creating 
printer-friendly versions of pages 
- Multiple style sheets: one for typography, layout, forms, tabels etc
  - link  in head 

## Chapter 3 (first part): “Functions, Methods, and Objects”
- **Function**: groups statements together to perform specific task. recycleable. 
- textContent - returns text content of specific element
- Parameters vs Arguments
  - Parameters are true values that will be used in the function
  - arguments are variables that hold real numbers that will be passed into the function
- Get more than one values out of function
  - return mutliple values in an array
  - when calling the values ex. getSize(0, 1, 2)[1] this calls the function then the [] will return value in the array at index 1
- immediately invoked function expression(IIFE)
  - place function in () then add () at the end before closing ) to call function immediately
- use anonymous and IIFE functions when needed once rather than repeatly called.
  - in event handlers, listeners
  - to prevent conflicts with like variables
- Variable scope
  - global: access anywhere on script, **use more memory** 
  - local: function level, canot be accessed outside function

## Article: “6 Reasons for Pair Programming”
- Driver: promgrammer who is typing, doesn't provide any direct inpt to computer
- navigator: uses words to guide driver but does not direct into to computer
  - think of big picture, converts to code, scans for typos, looks up solution and documnetation 
- Skills
  - listening
  - speaking
  - reading 
  - writing
- Improves efficiency, collaboration .learning, social skills, job interview readiness, work environment readiness