## Reading Class 10 

#### Understanding the JavaScript Call Stack

1. What is a ‘call’?
- invocation like a method invocation 
2. How many ‘calls’ can happen at once?
  - one at a time, calls will happen from top to bottom
3. What does LIFO mean?
  - last in, first out 
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
  - firstMethod
  - secondMethod(firstMethod)
  - thirdMethod(SecondMethod)
  - call thirdMethod()
  - the stack would be first, second, and third because the third method is invoked, which invokes the second method then the first method that is nested
5. What causes a Stack Overflow?
- **recursive function**: a function that calls itself 
- Every browser has a max stack call until it throws a stack error and calling a recursive function will throw a range error meaning the browser's stack has hit it's max meaning it is stack overflow
- too many stack errors in browser = stack overflow

#### JavaScript error messages

1. What is a ‘reference error’?
  - mismatched variable, hoisting d/t let and const, 
2. What is a ‘syntax error’?
  - code has something that can't be parsed d/t syntax
3. What is a ‘range error’?
  - declaring an object/data structure with an invalid length like giving an array of 0 a length of -1
4. What is a ‘type error’?
  - data type being accessed in incompatible 
5. What is a breakpoint?
  - an stopping place to evaluate your code when usng a debugger. Debugger tool will run everything before the line you use as a breakpoint and from there you can evaluate line by line as needed
6. What does the word ‘debugger’ do in your code?
  - debugger statement is added to a line in code to create a breakpoint

#### Bookmark and Review
**JavaScript errors reference on MDN**

#### things I want to know more about
- what are some things i can do with recursive functions

parts of an error message 
1. note if error was properly handled
2. type of error
3. call stack
