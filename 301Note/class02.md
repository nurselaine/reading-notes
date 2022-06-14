## Reading notes Class 02: State and Props

## React LifeCycle
- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
  - the render occurs before the componentDidMount during the mounting phase 
- What is the very first thing to happen in the lifecycle of React?
  - Mounting: this is when instances of components are being creating and inserted into the DOM 
- Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
  - constructor
    - this is called before mounting 
  - render
    - required method in class componenet: reads props and state when called 
  - componentDidMount
    - invoked right after component is mounted, good time to input anything that requires the components already in the DOM; also good to put setState
  - React Updates
    - anytime component/state updates, react re-renders
  - componentWillUnmount  
    - final stage when component is removed from DOM
- What does componentDidMount do?
  - Once component is rendered, this phase works for DOM manipulation and network requests as well as state changes which will re-render the page

## React State VS Props
- What types of things can you pass in the props?
  - An initializer, something to render, something that needs to change outside the component
- What is the big difference between props and state?
  - Props: like arguements to a function, what you want to initialize/render in your component. Handled outside a component and must be updated outside 
  - States: Handled inside a component, must be updated inside component
    - State is there for re-rendering and updating based on user interaction. Store information that will change in states
- When do we re-render our application?
  - whenever state updates 
- What are some examples of things that we could store in state?
  - form inputs like which option user selects or what the user inputs
- Key Ideas: Props are handled outside of components and passed into components to be used while States are handled and managed inside of components and ONLY inside. 

## Things I would like to learn more about
- I would like to know how to use props for functional components and better understand the differences passing props into a class component and a functional component 
- How do states get to update other components - While reading about the unidirectional data flow, I was wondering if a state from a child component trigger a state from the parent component to change? In a way, does that mean that states of different componenets interact with each other, so they're not ONLY involved inside their component?