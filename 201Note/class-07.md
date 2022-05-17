# Class 07 Reading Notes
## Domain Modeling

- Create conceptual model in code for specific problem
  - Model: describes various entities, attributes, and behaviors
- Object Oriented Model: entity that stores data in properties and stores behaviors in methods
- Constructor: needed to define between various objects
- Factory (constructor) Function: Function that can be used to create new properties for objects
  - objects created from this function are stored in variables
  - **this keyword** data inside parameters will be using this keyword
  - "Instantiate" declare new object using **new keyword** which creates new objects
  - then store inside variables

## Chapter 6: “Tables” (pp.126-145)

- Basic table structure
  - table: used to create table, content is written row by row
  - tr: indicates start of each row 
  - td: represent each table cell element
  - th: table headings nested inted tr (table row)
  - thead are headings of table 
  - tbody data of data should sit into body
  - tfoot footer of element
- Spanning Columns
  - use colspan attribute on th/td to select how many cells specified cell should run accross
  - rowspan attribute on th element can stretch down column specified amount

## Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

- constructor notation: new keyword and object constructor create blank object which properties & methods can be added
  - use dot /bracket notation to add methods & properties
- delete keyword: used to delete propery name | delete ojectName.property | clear vae of property objectName.property = ''
- Template functions: create objects with common properties, this.keyword is used instead of object name, template(constructor)  function is named with uppercase letter | function Factoryfunction: to help remind devs to use this keyword
- Create object using constructor function
  - let objectName = new constructorFunction('parameters', parameter, parameters..);
- Create Objects 
  - literal notation | define variable name = {} then add properties/methods via dot/bracket notation
  - object cnstructor notation: let name = new Object(); at properties/methods via dot/bracket notation or construction function
- this keyword: use this to show belonging to object
- Browser Object Model: objects that represent browser window
  - Window object: Top most object in BOM and contains other objects that provide info about the browser
- Global JS objects: Objects represents things that JS needs to create a model of
- DOM: represents model of current page
  - Document Object: topmost object in DOM, properties(title, lastModified, URL, and domain)
- Arrays are objects: set of key value pair (index-value)
- function are objects, callable: tell interpreter when execution is needed 
- JS treats every variable as an object 
- Rounding Decimals
  - tofixed() rounds to specified decimal places
  - toPrecision rounds to inidcated total number of digits 
- Math ObjectL properties and emthods for constants and functions
  - currently using Math.random
- Date object : to specify time and date of object

# Class 08 Reading
## Learn CSS - Layout
## Duckett HTML/CSS book: Ch. 15, “Layout” (again; repeat of Class 4 reading)