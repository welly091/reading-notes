Reading

What is a 'Controlled Component'?
  -When we use 'state' in a component to store and motify data, this component is called 'controlled component.'
  -For 'uncontrolled component', we use a 'ref' for handling data. A ref allows us to handle data by DOM itself. 
Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
  -We should wait to store the form's data into state when users submit the form so that we can update the data and re-render.
How do we target what the user is entering if we have an event handler on an input field?
  -Use event.target.value will show what the user entered in the input.

The Conditional(Ternary)Operator Explained
Why would we use a ternay operator?
  -Shorter and simplier version of if statement. Make the code look clear.
Rewrite the following statement using a ternary statement:
  ```
  x === y ? console.log(true) : console.log(false)
  ```
