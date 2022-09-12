## Class05 Reading Notes: Putting it all together

#### React Docs - Thinking in React

1. What is the single responsibility principle and how does it apply to components?
- Components should only be responsicble for ONE things which is known as the single responsibility principle
- a component should only handle one task, if it does more, then it should be refactored into smaller subcomponents
- organize the hierarchy of components as well!!
2. What does it mean to build a ‘static’ version of your application?
- first create a model of component hierachy that render the UI without functionality
- using this first model aka the static version, you can begin to add props so you know where your data lies and how you might pass one piece down/up the hierarchy
- DO NOT USE STATE while building the static version because it is reserved to allow components to interact aka data that changes 
- this version will render data and you will be done modeling the component hierarchy on the UI
3. Once you have a static application, what do you need to add?
- Identify the minimal representation of UI state - make UI interactive using state
- Gather what states the app needs be DRY (think of the absolute minimal rep of your state)
- Figure out if it state:
  1. is it passed in from a parent
  2. does it remain unchanged
  3. can you compute it based on another other state/props in component
-For each State:
  1. identify every component using that state
  2. find a common component to house that state(a higher level component would be a good owner)
  3. if no component is ideal to house the state: CREATE A NEW ONE!
- What are the three questions you can ask to determine if something is state?
 1. is it passed in from a parent
  2. does it remain unchanged
  3. can you compute it based on another other state/
How can you identify where state needs to live?
- Higher-Order Functions
  1. identify every component using that state
  2. find a common component to house that state(a higher level component would be a good owner)
  3. if no component is ideal to house the state: CREATE A NEW ONE!

#### Higher Order Function
What is a “higher-order function”?
- functions that operate by taking another function as an arguement or by returning a function
- Allows abreactions over actions and values
  1. functions that generate new function
  2. functions that change other functions
  3. functions that provide new types of control flow
    - pass in if and then => if (test) then()
- data processing 
Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
  - this function passes in an arguement, and uses that arguement to return a function m => m > n which will return either T or F
Explain how either map or reduce operates, with regards to higher-order functions.
- map transforms an array by applying a function to all of it's elements map.push(function(elements)) pass a function in a function aka higher order function
- reduce: takes in three parameters, combining function and a start value, and array. Initialize a value to hold all combined values of the array to the combine method with this value and each elem inside the array passed through

### [Things I want to know more about](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)
- Building react app top down vs bottom up: I want to make mock ups of this to get a better idea of organizing my apps

- Abstrction: hide details and give us the ability to talk about probelms at a higher level aka more abstract 