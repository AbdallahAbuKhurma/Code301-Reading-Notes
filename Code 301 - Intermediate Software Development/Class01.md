# Class 01 Notes

## Intro To React

* ReactJS offers graceful solutions to some of front-end programming’s most persistent issues, allowing you to build dynamic and interactive web apps with ease.

* React is a declarative, efficient, and flexible library for building user interfaces.

* Components :complex ULs from small pieces of code. we use components to tell React what we want to see on the screen. React will update and re-render the components when the data change.

* In JavaScript classes, we need to always call super when defining the constructor of a subclass. All React component classes that have a constructor should start with a super(props) call.

## Hello World (React Example)

ReactDOM.render(

# Hello, world

, document.getElementById('root') );

## Introducing JSX

### Why JSX?

* React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

* Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both.

* We split JSX over multiple lines for readability. While it isn’t required, when doing this, we also recommend wrapping it in parentheses to avoid the pitfalls of automatic semicolon insertion.

### Specifying Attributes with JSX :

* we use quotes to specify string literals as attributes :

* example : const element =

;

* also we can use curly braces to embed a javaScript expression in an attribute:

* example: const element = ;

## Rendering Elements:

* Elements are the smallest building blocks of React apps.

* the element describes what you want to see on the screen.

* React elements are plain objects, and are cheap to create.

* DOM takes care of updating the DOM to match the React elements.

* To render a React element into a root DOM node, pass both to ReactDOM.render().

* React elements are immutable. Once you create an element, you can’t change its children or attributes.

* React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.

## Components and Props:

* Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.

### Function and Class Components:

* The simplest way to define a component is to write a JavaScript function

* example: function Welcome(props) { return

# Hello, {props.name}

; }

* props : single object contain the JSX attribute and children of the user defined component.

### Composing Components

* Components can refer to other components in their output. This lets us use the same component abstraction for any level of detail. A button, a form, a dialog, a screen: in React apps, all those are commonly expressed as components.

* when you declare a component as a function or a class, it must never modify its own props.

* All React components must act like pure functions with respect to their props.

* Sources : hello-world introducing-jsx rendering-elements components-and-props
