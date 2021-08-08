# useState() Hook
>
## Review, Research, and Discussion

1. How does React differ from vanilla JS/HTML/CSS?\

        With React, we write HTML using JavaScript. We rely on the power of JavaScript to generate HTML that depends on some         data, rather than enhancing HTML to make it work with that data. Enhancing HTML is what other JavaScript frameworks         usually do.
        Vanilla JS is nothing but plain JS without any external libraries or frameworks. Using this we can build powerful and         cross-platform applications.
        React is a Javascript library used for building user interfaces. It allows us to make complex UIs from isolated pieces         of code called "components".
        In Vanilla JS, the code becomes very difficult to maintain if the application is large because in such cases the UI         needs to be updated regularly.

2. What is the primary difference between a function component and a class component?

        A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components.

## Document the following Vocabulary Terms

* Functional Components: are basic JavaScript functions, these are typically arrow functions but can also be created with the regular function keyword (the best practice). Sometimes referred to as “dumb” or “stateless” components as they simply accept data and display them in some form; that is they are mainly responsible for rendering UI.

* Children / Child Components: children allow you to pass components as data to other components, just like any other prop you use. The special thing about children is that React provides support through its ReactElement API and JSX. XML children translate perfectly to React children.

## Preparation Materials

### Hooks

“Hooks are an experimental proposal to React. You don’t need to learn about them right now. Also, note that this post contains my personal opinions and doesn’t necessarily reflect the positions of the React team”.

### Use Hooks

“when we write a function component, and then we want to add some state to it, previously you do this by converting it to a class. But, now you can do it by using a Hook inside the existing function component”.

### Using the State Hook

” In a function component, we have no this, so we can’t assign or read this.state. Instead, we call the useState”.
” The only argument to the useState() Hook is the initial state. Unlike with classes, the state doesn’t have to be an object. We can keep a number or a string if that’s all we need”.
example to get familiar with Hooks:

    import React, { useState } from 'react';
    
    function Example() {
      // Declare a new state variable, which we'll call "count"
      const [count, setCount] = useState(0);
    
      return (
        <div>
          <p>You clicked {count} times</p>
          <button onClick={() => setCount(count + 1)}>
            Click me
          </button>
        </div>
      );
    }

### Hooks at a Glance

“Hooks are functions that let you “hook into” React state and lifecycle features from function components. Hooks don’t work inside classes — they let you use React without classes. (We don’t recommend rewriting your existing components overnight but you can start using Hooks in the new ones if you’d like”.

## Resources

[making sense of hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)

[the state hook](https://reactjs.org/docs/hooks-state.html)

[hooks api](https://reactjs.org/docs/hooks-overview.html)

[hooks api reference](https://reactjs.org/docs/hooks-reference.html)
