# Class 05 Reading Notes
<hr>

## Chapter 3: “Object Literals” (pp.100-105)
<hr>
- Constructing an Object, user new keyword
  - let hotel = new Object(); or let hotel = {[properties and methods]}
- Object: groups together variables and functions that models something in the real world
  - variable become properties
  - function become methods
  - key and value model
- literal notation: used to create obejcts, declare object then initialize with {} curly braces
- dot notation to access methods and properties within object

## Chapter 5: “Document Object Model” (pp.183-242)
<hr>
- DOM tells browser how to create model of HTML AND how JS can interact with webpage content
- DOM is separate set of rules
  - browser loads webpage & creates **model** of page in memory
  - DOM tells browser how to structure this **model** via **DOM Tree**
    - Model = DOM Tree: is made up of objects and stored in browser memory
      - Document node: represents entire page
      - Element nodes and elements are interchangeable | DOM is working with node that represents element
  - DOM interacts with objects via methods and properties to update borwser model
- API (Application Programming Interface): alternate term for DOM, 
  - interface: allows programs/scripts to interact with each other
  - DOM can ask browser about current page then tell browser to update what user sees
<img src="dom-tree.png" alt="DOM Tree" style="float: left">
  - Attribute nodes in pink and Text notes in purple
- How to use DOM Tree:
  1. Access the Elements (refer to page 188 for various element access commands)
    - most popular is getElementById([id value]); and querySelector()
  2. Work with selected elements
- **Find the quickest way to access element to make page seem fast/more responsive**
- Returns 1+ elements: Methods faster than querySelectorAll()
  - getElementsByClassName, getElementsByTagName
- getElementById: quickest/efficient way to access one element using id attribute
- **querySelector**: Not support by older browsers, **parameter is CSS selector** to accurately target various elements querySelectorAll(li.hot);
- Nodelists: dom queries that return 1+ elements, elements stored in list are in same order they appear in HTML
  - Select one element from nodelist or loop through each item in nodelist (.map)
  - Live nodelist: list updates each time page updates, methods using getElementBy... return live nodelists and are faster than static
  - static nodelist: not updated with each page update. querySelector returns static nodelists 
  - item([index]) returns an individual node from nodelist | Array syntax faster than item()
- Array Syntax: variableName[index]
-  White space = text node in some browsers
- Be aware, when elements are mixed with other elements, selectors are more likely to target the container
  - document.getElementById('id').firstChild.nextSibling.nodeValue; li with em nested inside text
= .replace() replaces text value & nodeValue returns value of element
  - .textContent to collect or update text | variableName.textContent; returns value 
    - innerText property: avoid d/t unsupportive browsers, does not return values with hidden CSS attribute, **slower to retrieve content**
- DOM maniputlation: DOM methods that allow creation of elements and text nodes to attach/remove to DOM tree
  1. use DOM method to create new content one at a time then store in varianle
  2. Use another DOM method to attach variable to DOM tree
  3. Remove element using DOM method
  - innerHTML: returns content of elements as a string 
    - Cross-Site Scripting Attacks(XSS): attacker places malicious code into site and gains access to DOM, cookies, info identifying users
      1. Ensure input characters that are valid
      2. validate server before using user content in database
      3. Do not use HTML from untrusted sources
  - Create an element: createElement(), createTextNode() with appendChild
    1. create new element then store in variable let newEl = document.createElement('li')
    2. Create text node and store in variable let newText = document.createTextNode('hello world');
    3. attach text node to new element newEl.appendChild(newText)
    4. Position where new element should be added let position = document.gtElementByTagName('ul')[0]
    5. Insert new element position.appendchild(newEl);
  - Remove an Element | removing element also remove children of element
    1. Store element to be removed in variable let removeEl = document.getElementByTagName('li')[3]
    2. Store parent of elelment in variable let containerEl = removeEl.parentNode;
    3. remove element from containing element containerEl.removeChild(removeEl);
      - removeChild() used on variable that holds the container node and passes in element being removed
- Attribute methods: getAttribute, hasAttribute, setAttribute, and removeAttribute  
  - good practice: check whether attribute exists, to save on resources


## what I would like to learn:
- I would like to learn the best ways to access nodes to build an efficient and fast webpage
- I want to apply all the DOM methods and selectors to better understand which ones to use depending on the situation
