Life cycle is another important core topic to React. It defines a *life* of a component.

(Mounting ...)                                            
constructor -> getDerivedStateFromProps -> render -> componentDidMount -> UNSAFE_componentWillMount

(Updating...)
getDerivedStateFromProps -> shouldComponentUpdate -> render -> getSnapshotBeforeUpdate
-> componentDidUpdate -> UNSAFE_componentWillUpdate -> UNSAFE_componentWillReceiveProps

(Unmounting...)
componentWillUnmount

Reading questions:
1. Based of the diagram, what happens first, the render or the componentDidMount?
    -> render goes first.
2. What is the very first thing to happen in the lifecycle of React?
    -> Constructor is called first.
3. Put the following things in the order:
    -> Constructor -> render -> componentDidMount -> React Updates -> componentWillUnmount
4. What does componentDidMount do?
    -> This method is invoked immediately after a component is mounted. This is the place where you can put subscriptions. 
       You have to be careful while putting any function that causes rerender like setState().
Video questions:
1. What types of things can you pass in the props?
    -> Any data type
2. What is the big difference between props and state?
    -> Props is the thing you want to pass to another component. State is the thing you want to keep inside in a component.
3. When do we re-render our application?
    -> If state is changed, it will re-render the application.
4. What are some examples of things that we could store in state?
    -> User input, check box, select box... 
