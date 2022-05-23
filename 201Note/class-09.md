# Class09 Reading

## Chapter 7: “Forms” (p.144-175)
- forms: box that allows users to perform functions
- Anatomy of Form: 
  - Text Box: for input, password input, and multiline input
  - choices: radio buttons, checkboxes, and dropdown boxes
  - submitting forms: submit buttons, image buttons, and file uploads
- Form patho
  1. user fills out form
  2. name of each form control is sent to server with value user input/selects
  3. server processes info using programming language/store info in database
  4. server creates new page to send back to browser based on info recieved 
- Building a form
  1. form tag: parent of form controls and carries 
  2. **action attribute** (mandatory): url for page on server that will receive information in the form when submitted 
  3. method: get or post, needed to send forms
    - get method: values from form are added to end of URL specified in action attriubte | good for short forms (Search boxes - just retrieving data from web server). **default** method to send data
    - post method: values are sent in a HTTP header | use for file uploads, long form, sensitive data, add/delete info from database
  4. id attribute: used to distinct form from other elements on page 
  5. input element: used to create different form controls
    - type attribute: value is the type of input (text); button types(radio, checkbox)
      - password types creates text box that accept single line input with characters blocked out
      - date: gives user options to choose date input 
      - email: HTML will validate correct data has been inputed 
      - type="url" used when user inputs websites
      - search value allows user to search queries 
    - name attribute: tells server which form control is sent along with info user enters
      - why? user enters info into form, server needs to know which form control data was entered into. login forms, a username form control would need a different name attribute than a password name attribute because the server needs to know the difference 
    - max-length attribute: limit characters user may enter
  6. textarea element: creates multiline text input | Text inbetween open/close tags
    - CSS to control width and height
    - cols & rows attribute: to indicate how wide / how many rows needed
  7. Select element: creates drop down list to pick from | works well with long lists of options
  - Option elements are nexted inside with value attribute
  - selected attribut: indicate the option that should be selected when page loads/default option will be the first option on the list
  - size attribute: value is number of options to show user from dropdown box
  - multiple attribute: allows users to select multiple options from list 
- input element: allows users to input files and submit uploads | use type: file attribute
  - method attribute MUST have value of form 
  - use type attribute for submit function 
8. images for submit button , use input element with type attribute "image"
9. button element: can nest img tag inside add width, height attributes 
  - type: hidden attribute useful to webpage authors to add values to forms that users cannot see
10. Label elements: form control for vision impared users
  - Wrap around input element 
  - use for attribute and keep separate from form control
    - for attribute states which form control label belongs to then user can click on label or button
11. Best places to put form controls: Above/left for text inputs, text areas, select boxes, and file uploads
- right side: individual check boxes and radio buttons
12. Feildset element to group related form controls
  - Legend element: after feildset element, contains caption to identify purpose of form controls (contact details)
13. form validation

form with action attribute
- feildset
  - legend to describe form purpose
    - label & input elements with type, name and size attributes
      - put breaks in between each label element


## Chapter 14: “Lists, Tables & Forms” (pp.330-357)
- list-style-type: none, disc, circle, and square options and images (url="url")
- ol have list-style-type : decimal, decimal-leading-zero, lower-ramon, upper/lower alpha
- Border-spacing: control distance between adjacent cells in table: px
- border-collapse: collapses borders of table into single border
- **page 344 styling for forms**

## Chapter 6: “Events” (pp.243-292)
- Interactions create events
- Events trigger code: fired/raised which trigger a function/script
  - Look up list of event types
- cose responds to users
 1. Event Handling: Select Element script should respond to (i.e. button)
  - One function per event handler | element.event = functionName; **do not put parenthesis** bc code should run when event is triggered which is why () is omitted
  - use "on" for event handler calls
  2. Binding: (event to dom) indicate type of event that will trigger response 
    - binding(3) event handlers and event listeners
  3. Code: Write function for event handler that instructs what will occur
- Flow: matters when event handlers on element and one of it's ancestors/descendant elements
- event object(e): tells info about event and element it occured on, passed into handler/listener
- Event delegation: multiple event listeners can slow webpage
  - event flow allows parent element to listen for events in children elements
    - use target.property to find which child event occured on
  - rule: attach event listener to container (delgating listener to parent
- event methods
  - preventDefault() stops default behavior to keep user on same page 
  - stopPropagation() stops event handler from "bubbling" up to ancestors ???
- this: refers to owner of function 

- event types 
    - UI Events: Load, unload, error, resize, scroll
    - Keybord events: keydown (event will repeat while key is depressed), key up (user releases key), keypres (Character is being inserted - also repeats event while depressed)
    - Mouse events: click, dblclick, mousedown, mouseup, mousemove, mouseover (mouses over an element), mouseout 
        - mouseover and mouseout commonly used to change appearance of boxes/switch images as user rolls over them - use CSS to change appearance of element
        - mousedown and mouseup and different to create drag and drop features/ game controls
    - focus events: occurs when element gains/loses focus, fous: focus in/blur: focus out
    - form events: input, change, submit, reset, cut, copy, paste, select
    - mutation event: DOM structure has been changed by script: DOMSubtreeModified (change has been made to document)
- Triggering event
   1. select element node that will respond
    2. pick an event and bind node to event listener
    3. create event handler function that will create an action 
- Event listeners: element.addEventListener('event type', '(callback)-function name', [boolean])
    - bind node to variable
    - use variable and dot notation to add event listener 
    - pass in three parameters into event listener
        - first param is event name, second param is start of anonymous function, third param is event flow boolean
- Event Flow: order in which events fire (event listeners act on all related/nested nodes)
    - Events flow in two directions 
        1.  Event bubbling: Start from inner node then flows outwards to least specific node
        2. Event Capturing: start from outermost node (least specific) to flows to inner most node
- Boolean flow param: true = capturing (outward in) & false = bubbling (inward out)
- Event Object: provides info on event and element event occurs on 
- FYI: adding event listening to each element uses a lot of memory and slows down performance
    - resolution: place event handles in containing elements and use event object target property to find which child event occurred on
- Default behavior: 
    - preventDefault(): keeps user on same page 
    - stopPropagation: stop event from bubbling up to parent elements after event has been handled 
- UI events: raised when user interacts with browser window (page loaded, browser window being resized)
   - attach event listen for UI events to browser window
    - Event triggers: load (webpage finishes loading), unload (before user leaves page), resize, error(JS error), scroll(user scroll up.down)
        - Ex. load event: fires when page finishes loading, a form with input for username could be attached to load listener. Attach load event to window so on event window will execute function that causes window to focus on username input of form. without load listener, browser's focus would not be on username input
- Event Object and mouse events: 
    - screenX or screenY properies, indicate position of cursor within entire monitor (L to R)
    - pageX and pageY indication cursor position. Top of page may be outside viewport, so page and client coordinate may be different
    - clientX and clientY: cursor position in browser's viewport, scrolling up/down does not affect client's coordinates
- Keyboard events: event object returns which key was pressed using keycode property