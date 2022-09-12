## Reading notes Class 04: Reacts & Forms

#### Forms
1. What is a ‘Controlled Component’?
  - HTML elements that maintain their own state (like form), combine with React state, so the react component now controls what happens to the element 
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
  - Update the state after every keystroke - to keep react state always up to date to visually show the user what is being typed (onchanged) the state will update onChange value which will display each keystroke to the user. Else no keystroke would be displayed until submit is pressed
3. How do we target what the user is entering if we have an event handler on an input field?
  - use event object and in the input field have a value property 

#### Ternary Operator
1. Why would we use a ternary operator?
  - ternary operators are conditionals that are refactored to be shorter and give the program two options to choose, T or F
2. Rewrite the following statement using a ternary statement:
- x===y ? console.log(true) : console.log(false)

### What I want to know more about
- Why would I use an inline conditiona && expression if truth always results to expression? (nevermind)
- toggling events and states. in the example for conditional rendering, should the warning state be true?
- when it is true, the button will display 'hide' and the toggle event handle will set the state to false when the user clicks on the button then the process starts again?

