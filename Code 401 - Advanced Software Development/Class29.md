# Advanced State with Reducers
>
## Review, Research, and Discussion

1. How can we ensure that an effect hook runs only once?

        React has a built-in hook called useEffect. Hooks are used in function components. The Class component comparison to useEffect are the methods componentDidMount , componentDidUpdate .

2. Can useState() update more than one state variable at the same time?

        we could do one setState call and there will only be one render. Unlike the setState in class components, the setState returned from useState doesn’t merge objects with existing state, it replaces the object entirely.

3. Is useState() synchronous?

        useState and setState both are asynchronous

## Document the following Vocabulary Terms

* State Hook The useState() is a Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries.

* Component Lifecycle the series of methods that are invoked in different stages of the component’s existence. The three phases are: Mounting, Updating, and Unmounting.

## Preparation Materials

How does useReducer work?
useReducer is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.

useReducer is one of the additional Hooks that shipped with React 16.8. An alternative to the useState Hook, it helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux or MobX — indeed, it can sometimes be an outright better option.

There are three main building blocks in Redux:
A store — an immutable object that holds the applications state data
A reducer — a function that returns some state data, triggered by an action type.
An action — an object that tells the reducer how to change the state. It must contain a type property, and it can contain an optional payload property const initialState = { count: 0 }
const [state, dispatch] = useReducer(reducer, initialState) The reduce() method in JavaScript executes a reducer function on each element of the array an and then returns a single value.

There are two different ways to initialize the useReducer state.
The simplest way is to pass the initial state as a second argument const [state, dispatch] = useReducer( reducer, {count: initialCount} );

You can also create the initial state lazily To do this, you can pass an init function as the third argument. The initial state will be set to init(initialArg)

## Resources

[useReducer hook](https://reactjs.org/docs/hooks-reference.html#usereducer)

[Ultimate Guide to useReducer](https://blog.logrocket.com/guide-to-react-usereducer-hook)
