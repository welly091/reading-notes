Reading

What is a 'Controlled Component'?
  -When we use 'state' in a component to store and motify data, this component is called 'controlled component.'
  -For 'uncontrolled component', we use a 'ref' for handling data. A ref allows us to handle data by DOM itself. 
Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
  -Not use about this one. I guess we update the state with users responses as soon as possible so that we keep the data in state and the component got re-rendered.
How do we target what the user is entering if we have an event handler on an input field?
  -Use event.target.value will show what the user entered in the input.

The Conditional(Ternary)Operator Explained
Why would we use a ternay operator?
  -Shorter and simpler version of if statement. Make the code look clear.
Rewrite the following statement using a ternary statement:
  ```
  x === y ? console.log(true) : console.log(false)
  ```
