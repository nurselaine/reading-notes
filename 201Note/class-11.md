# Class-11 reading notes

## Chapter 16: “Images” (pp.406-427)
- Float: used to align images and add margin to ensure text doesn't touch image
- img are inline by default, change display to block
- Centering img
  1. display img as block and use text-align property to center in containing element
  2. on img element, set R and L margin to auto
- Background img: allows to place image behind any HTML element, will repeat to fill container by default and last thing on page to load
  - FYI: that larger the img file the longer the loading time
  - Properties: 
    - Background repeat(horizontal and vertical): repeat-x, repeat-y, fixed, scroll, and no-repeat
    - background-position (works when img is not repeated, used to specifiy where to position img on browser window): ex. left center, center top, etc and pair with px or % which represent distance from top left corner of window 
  - **Shorthand** ex (background: #ffffff url("img/image.jpeg") no-repeat top right)
    1. background-color
    2. background-image
    3. bakcground-repeat
    4. background-attachment
    5. background-position
- Image rollovers: when user mouses over element, element's style changes 
  1. set background image for element to have three different styles of same button 
- img sprites: single image is used for sevela parts of interface, improves loaiding time for browser
- anchor element is inline element, set display to inline block to specify width and height 
- **Overlay text on background img**: img must be low contrast
  - high contrast: marjority of img
  - low contrast: use image editing apps to manually adjust contrast
  - alt: overlay text on image with high contrast (it's ugly)
  

## Chapter 19: “Practical Information” (476-492)

## This MDN article on audio and video elements
- Creating a video 
- HTML
  - video element 
    - nest source element with one audio and one video 
  - Div to handle controls
    - Buttons: 
      - Play and stop buttons
      - rewind and forward buttons
      - Attributes: class, data-icon (defining what icon should be shown on each button), aria-label(provide description of each button and used by screen readers for visually impaired)
    - nested div inside controls (timer div to report elapsed time)
      - create an empty div
      - timer: create inline element like span with value 00:00
- CSS
  - refer to doc for reference styling
  - @font-face black to import custom web font: cuts down on HTTP requests + icon img downloads
- JavaScript
  - create new js file (custom-player.js)
  - bind controls and media elements to variables using query selectors: hld references to all objects needing manipulation
  - remove defualt broser controls from video
    - add media.removeAttribute('controls')
    - controls.style.visibility = 'visible'
  - Functions: 
    - playPauseMedio(): Add event listener to play reference variable, event type is click and pass in playPauseMedia function
      - inside function, use if/else to distinguish action for pause and play
    - stopMedia(): add a click and ended event with stopMedia() function
      - use pause() in method and set currentTime to 0 so media jumps to starting time
    - mediaBackward/Forward(): click events with two different functions
      - create global variables for back and forward intervals
