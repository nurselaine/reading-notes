## Class 09 Reading Notes

#### Functional Programming Concepts

1. What is functional programming?
  - a programming style of building the structure and elements of applications 
  - it involves computation and avoid changing state and mutable data
2. What is a pure function and how do we know if something is a pure function?
  - a pure function will return the same result of the arguments and doesn't cause any side effects
    - side effects: modifying global object or a parameter passed (mutability is discouraed)
  - Using global objects make functions impure 
3. What are the benefits of a pure function?
  - makes code easier to test 
4. What is immutability?
  - unchanging over time and unable to change
  - create a new object with new values if needed 
5. What is Referential transparency?
  - the function always produces the same result for the same input 
    - pure functions + immutable data = referential transparency
Videos

##### Node JS Tutorial for Beginners #6 - Modules and require()

1. What is a module?
  - a way to organize node.js applications into functional parts. Each module accounts for a specific function
2. What does the word ‘require’ do?
  - it functions as an import for another module 
3. How do we bring another module into the file the we are working in?
  - global object in node - require(./'pass a string of a path to module required in file') do not include .js/.file type when calling
4. What do we have to do to make a module available?
  - in the module you want to use in another module - at the bottom say:
    - module.export = what we want to make available outside the function like a function name 