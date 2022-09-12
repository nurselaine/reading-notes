## Reading notes Class 03: Passing Functions as Props

### Lists and Keys
1. What does .map() return?
- .map is a method that returns a new array (with changes made using the callback function passed into the method)
2. If I want to loop through an array and display each value in JSX, how do I do that in React?
- To render mutliple componenets use curly braces 
- Use a forEach or map through an array then return the JSX element with specified attributes and values
- make sure to include the array with elements being pushed inside in the parent element to render
4. Each list item needs a unique key.
5. What is the purpose of a key?
- Keys help react identify which items have changed, added, or have been removed
- Common to use IDs from data as keys to keep each key unique (if not ID then use index, make sure order of items do not change if uses indexes)
- Extractung using Keys
  - Keys need to be unique among sibling, but not between two global arrays
- Embedding an espression, inside JSX, use curly braces and input Javascript expressions

The Spread Operator
1. What is the spread operator?
  - allipsis of three dots ... which is used to exand an iterable object into a list of arguements
  - Added with AS6
  - Takes an array and spreads each element into separate arguements
2. List 4 things that the spread operator can do.
  1. spread array elements into separate arguements
  2. Copying, concatenating, and combining an array
    - Copying: arr = [1,2,3,4]; to newArr = [...arr]
    - concatentating: newerArr = [...arr, ...newArr]
  3. Using Math Functions
    - Math.min([...1,2,3])
  4. Adding items to a list, adding state to component, combinig objects
3. Give an example of using the spread operator to combine two arrays.
  - concatentating: newerArr = [...arr, ...newArr]
  - combining: arr[1] newArr[2,3,4, ...arr]
4. Give an example of using the spread operator to add a new item to an array.
  - arr[1,2,3] newArr[...arr, 4]
5. Give an example of using the spread operator to combine two objects into one.
  - obj{key1: value1} obj2{key2: value2} =>
  - newObj = {...obj,...obj2} => key1: value1, key2: value2
- FYI: using spread will create a new reference which can help when reassigning the original array elements, the spread array will remain unchanged

#### How to pass functions between components
In the video, what is the first step that the developer does to pass functions between components?
- creates a function to pass into the child component which is called when state changes
In your own words, what does the increment function do?
- this function takes in a key arguement that identifies the person component then takes the count property from that person to update the value of count
How can you pass a method from a parent component into a child component?
- Pass in props associated with properties in parent component that will trigger a state change
- pass method as a property that will be passed down to child component
How does the child component invoke a method that was passed to it from a parent component?
- child component has a state that can be change

### Things I want to know more
- What's a good instruction set to follow when learning how to pass functions and create events/event listeners between parent and child components