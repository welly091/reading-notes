What is the single responsibility principle and how does it apply to components?
  - It means that each component does one thing only. If a components have many things to do, break down the code and create more sub-components to do those jobs.
What does it mean to build a 'static' version of your application?
  - Build a static version means that you build similar app only use props and render() methods but no states.
Once you have a static application, what do you want to add?
  - Add a data model so that the static version app can render it.
What are the three questions you can ask to determine if something is state?
  - Is it passed in from a parent via props? 
  - Does it remain unchanged over time?
  - Can you compute it based on any other state or props in your component? 
  If you can yes to one of these three questions, it is not state.
How can you identify where state needs to live?
  -Identify every component that renders something based on the state.
  -Find a common owner component.
  -Either the common owner or another component higher up in the hierarchy should own the state.
  -If you can't find a component where it makes sense to own the state, create a new one to hold the state.

Higher-Order Functions:
What is a higher-order function?
  - Functions that operate on other functions- taking them as arguments or by returning them- are called higher-order functions.
Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
  - Create a new function that takes 'm' as a parameter, and return that new function.
Explain how either map or reduce operates, with regards to higher-order functions.
  - 'map' iterate the original array and modifies those elements and return a new array.
  - 'reduce' will take an initial value and will go throw each element in an array and add on each value to it. Every time the value is updated, the value will be stored as an 'accumulator'. When the adding process is over, it will return the accumulator value.
  - Both map and reduce are higher-order functions because they take another function as an argument and to help us to get the result we want.
