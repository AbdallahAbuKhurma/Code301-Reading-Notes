# Redux - Asynchronous Actions
>
## Review, Research, and Discussion

1. How granular should your reducers be?

        many reducers is better than only a few or just one. and in Redux there is combineReducers method to combine these reducers .

2. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

        Not sure, I would guess con as it gets messy and actions need to get filtered through.

3. Name a strategy for preventing the above?

        thunk middleware or maybe you have to be more specific when you named the reducers!.

## Document the following Vocabulary Terms

* **store:** is a state container which holds the application’s state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer. Let us see how we can create a store using the createStore method from Redux.

* **combined reducers:** a helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object.

## Preparation Materials

### Async actions

* There are two very popular middleware libraries that allow for side effects and asynchronous actions: Redux Thunk and Redux Saga. In this post, you will explore Redux Thunk.

* Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation.

* Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.

* The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.

### Thunk middleware

With a plain basic Redux store, you can only do simple synchronous updates by dispatching an action. Middleware extends the store’s abilities, and lets you write async logic that interacts with the store.

Thunks are the recommended middleware for basic Redux side effects logic, including complex synchronous logic that needs access to the store, and simple async logic like AJAX requests.

### Redux Thunk

By default, Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects. Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers.

There are two very popular middleware libraries that allow for side effects and asynchronous actions: Redux Thunk and Redux Saga. In this post, you will explore Redux Thunk.

Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation.

Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.

## Resources

[async actions](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)

[thunk middleware](https://github.com/reduxjs/redux-thunk)

[redux thunk](https://www.digitalocean.com/community/tutorials/redux-redux-thunk)
