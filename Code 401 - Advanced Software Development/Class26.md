# Component Based UI
>
## Review, Research, and Discussion

**Name 5 Javascript UI Frameworks (other than React)**

1. Ext JS by Sencha.

2. Angular.

3. Vue.

4. Ember.

5. Svelte 3.

**What’s the difference between a framework and a library?**

The technical difference between a framework and library lies in a term called inversion of control. When you use a library, you are in charge of the application flow. You choose when and where to call the library. When you use a framework, the framework is in charge of the flow. It provides you with a few places to plug in your code, but it calls the code you plugged in as needed. Framework is often more restrictive and generally have a more set of rules.Whereas, Library is not bounded by many rules.

## Document the following Vocabulary Terms

**Rendering:**

Rendering is a process that is triggered by a change of state in some component of your application, when a state change occurs React: It will collect from the root of your App all the components that requested a re-render because their state or their props changed.

**Templates:**

React templates are sets of ready-to-use parts of code built using React technology for the development of dynamic user interfaces. React templates may contain full-fledged pages with a pre-built design, component compositions, stand-alone components, styling (like fonts, colors theme effects, background styles, icons), plugins, widgets, libraries

**State:**

What is State? The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.

## Preparation Materials

### JSX

* JSX produces React “elements”.

* React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

* React separates concerns with loosely coupled units called “components” that contain both.

* React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code.

* It also allows React to show more useful error and warning messages.

* You can put any valid JavaScript expression inside the curly braces in JSX.

### Rendering Elements

Let’s say there is a < div> somewhere in your HTML file,We call this a root DOM node because everything inside it will be managed by React DOM. Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.

## Updating the Rendered Element

* React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time. With our knowledge so far, the only way to update the UI is to create a new element and pass it to ReactDOM.render().

* It calls ReactDOM.render() every second from a setInterval() callback. React Only Updates What’s Necessary:

* React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.

## Resources

[react hello world](https://reactjs.org/docs/hello-world.html)

[introducing JSX](https://reactjs.org/docs/introducing-jsx.html)

[rendering elements](https://reactjs.org/docs/rendering-elements.html)
