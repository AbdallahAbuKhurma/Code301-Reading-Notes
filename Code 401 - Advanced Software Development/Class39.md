# Redux - Additional Topics\
>
## Review, Research, and Discussion

1. What’s the best practice for pre-loading data into the store (on application start) in a Redux application?

        The most ‘redux-like’ way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.

2. When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

        That will dispatch the response data to your action which will send the data to the reducer

## Document the following Vocabulary Terms

* **Middleware:** middleware allows for side effects to be run without blocking state updates. We can run side effects (like API requests) in response to a specific action, or in response to every action that is dispatched (like logging).

* **Thunk:** thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation.
Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.

## Preparation Materials

### Redux Toolkit (RTK)

Redux Toolkit is our official, opinionated, batteries-included toolset for efficient Redux development. It is intended to be the standard way to write Redux logic, and we strongly recommend that you use it.

It includes several utility functions that simplify the most common Redux use cases, including store setup, defining reducers, immutable update logic, and even creating entire slices of state at once without writing any action creators or action types by hand. It also includes the most widely used Redux addons, like Redux Thunk for async logic and Reselect for writing selector functions, so that you can use them right away.

The Redux core library is deliberately unopinionated. It lets you decide how you want to handle everything, like store setup, what your state contains, and how you want to build your reducers.

This is good in some cases, because it gives you flexibility, but that flexibility isn’t always needed. Sometimes we just want the simplest possible way to get started, with some good default behavior out of the box. Or, maybe you’re writing a larger application and finding yourself writing some similar code, and you’d like to cut down on how much of that code you have to write by hand.

**Redux Toolkit was originally created to help address three common concerns about Redux:**

1. Configuring a Redux store is too complicated

2. I have to add a lot of packages to get Redux to do anything useful

3. Redux requires too much boilerplate code

### Redux Toolkit includes

**configureStore():** wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.

**createReducer():** that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements. In addition, it automatically uses the immer library to let you write simpler immutable updates with normal mutative code, like state.todos.completed = true.

**createAction():** generates an action creator function for the given action type string. The function itself has toString() defined, so that it can be used in place of the type constant.

**createSlice():** accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.

**createAsyncThunk:** accepts an action type string and a function that returns a promise, and generates a thunk that dispatches pending/fulfilled/rejected action types based on that promise

**createEntityAdapter:** generates a set of reusable reducers and selectors to manage normalized data in the store The createSelector utility from the Reselect library, re-exported for ease of use.

## Resources

[Redux Toolkit (RTK)](https://redux-toolkit.js.org/)

[Tutorial](https://redux-toolkit.js.org/tutorials/overview)
