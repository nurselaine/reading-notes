# Reading 01: Introduction to React & Components

## Component Based Architecture
- the focus of breaking down an application into functional pieces that represent communicating parts of a whole
- **Component reusability** - primary function of components is to **encapsulate** functionality and behaviors
- Resuability: Reduces time in market and development costs & increased reliability 
- Component: a reusable function that intended to interact with other components (each component enapsulates certain functionality) 
- Views of a Component
  - object-oriented view: component is viewed as a set of 1+ classes
  - conventional view: functional element that possesses the logic and data structures for the compoennt to be invoked and data to be passed 
  - process-related view: building from existing components maintained in a library 
    - UI components: grids, buttons/controls
    - Resource intensive components: use Just-in-time approach
    - invisible components: provided in enterprise business and web applications 
- Component Characteristics: 
  1. Reusability: usable in different situations and applications
  2. Replaceable: Freely substitued with other components
  3. Not context specific: designed to operate in different environments
  4. extensible: can be extended from existing components to provide new behavior
  5. encapsultaed: allows user to call it's functionality without exposing details of internal processes/interval variables and states
  6. independent: designed to have minimal dependencies on other componenets
- Component based designs: Use a graphical/text-based diagram
  - design classes needed for infrastructure, define which classes will be reusable and which are not
  - defines each components interface and the data types/structures needed to build them
  - define data sources(databases/files) and identifies which class will manage them
  - improves the maintenance and evolution of building the application

## What is Props and How to use it in React
- Props: properties that represent data that can be passed from one component to another in a **unidirectional flow**
- Data coming from parent components should not be changed by child components: **props data is immuntable (read-only)**
- Passing a Prop
  1. define an attribute and it's value(data)
  2. Pass it to child component by using "props"
    - for regular components: pass in "props" and refer to property as : **props.variableName** utilize dot notation
  3. render the props data


## Review
#### Pass data through Props
#### Rendering elements
### JSX
#### Components & Props

## Things I want to know more about
- How do you come up with component level designs? How can I plan out an entire roadmap of my application 
