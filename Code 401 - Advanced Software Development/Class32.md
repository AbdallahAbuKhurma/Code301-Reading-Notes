# Context API - Behaviors
>
## Review, Research, and Discussion

1. When you have multiple contexts, what component type should you use (class/function) and why?

        The difference is pretty obvious. Class components are ES6 classes and Functional Components are functions. The only constraint for a functional component is to accept props as an argument and return valid JSX.

2. What are some good use cases for using the Context API for global state?

        Stripe : Stripe is one of the most successful and best known API-driven businesses.
        Ebay : Unlike the previous companies, eBay didn’t start out with the intent of being API-driven.

3. How can you best test context?

        The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).

## Document the following Vocabulary Terms

* **context:** Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

* **useContext():** hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”.

* **static context:** If you are using the experimental public class fields syntax, you can use a static class field to initialize your contextType.

## Preparation Materials

### Context api

Context provides a way to pass data through the component tree without having to pass props down manually at every level and In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

Before You Use Context Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult and If you only want to avoid passing some props through many levels, the component composition is often a simpler solution than context.

### Context.Provider

All consumers that are descendants of a Provider will re-render whenever the Provider’s value prop changes. The propagation from Provider to its descendant consumers (including .contextType and useContext) is not subject to the shouldComponentUpdate method, so the consumer is updated even when an ancestor component skips an update.

Changes are determined by comparing the new and old values using the same algorithm as Object.is.

### Context.Consumer

A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component.

Requires a function as a child. The function receives the current context value and returns a React node. The value argument passed to the function will be equal to the value prop of the closest Provider for this context above in the tree. If there is no Provider for this context above, the value argument will be equal to the defaultValue that was passed to createContext().

## Resources

[context api](https://reactjs.org/docs/context.html)

[hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)

[react context links](https://github.com/diegohaz/awesome-react-context)
