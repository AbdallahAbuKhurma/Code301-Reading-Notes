# Application State with Redux
>
## Review, Research, and Discussion

1. What are the advantages of storing tokens in Cookies vs Local Storage?

    * easier to retrive and edit
  
    * easier to clean or reset
  
    * cookies data will be sent over each request which is great to authentication and authorization on the previous one.

2. Explain 3rd party cookies:

        cookies that save in the browser via 3rd party sites like google and trackers that we uses there services in our website but not directly by us.

3. How do pixel tags work?

        The tracking pixel URL is the memory location on the server. When the user visits a website, the image with the tag is loaded from this server.

## Document the following Vocabulary Terms

* **cookies:** small bit of data stored on a user’s computer by the web browser while browsing a webiste, designed to be reliable mechanism for websites to remember stateful information or to record the user’s browsing activity

* **authorization:** is a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs, data and application features

* **access control:** Component of data security that dictates who is allowed to access and use company information and resources. Through authentication and authorization, access control policies make sure users are who they say they are and that they have appropriate access to company data

* **conditional rendering:** In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application. Conditional rendering in React works the same way conditions work in JavaScript

## Preview

1. Which 3 things had you heard about previously and now have better clarity on? context

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo? redux

3. What are you most excited about trying to implement or see how it works? its the redux week finally

## Preparation Materials

### Why use Redux?

Redux allows you to manage your app’s state in a single place and keep changes in your app more predictable and traceable. It makes it easier to reason about changes occurring in your app.

### how to use Redux in react

1. create store as we create context

2. pass store and context to provider

3. imported as context exactly

### How Redux works

* There is a central store that holds the entire state of the application. Each component can access the stored state without having to send down props from one component to another.

* There are three building parts: actions, store, and reducers.

## Fundamentals of Redux

1. State management is absolutely critical in providing users with a well-crafted experience with minimal bugs.

2. Redux provides a solid, stable, and mature solution to managing state in your React application.

3. Redux can transform your application from a total mess of confusing and scattered state, into a delightfully organized, easy to understand modern JavaScript powerhouse.

4. Redux is a predictable state container for JavaScript apps.

5. It helps you write applications that behave consistently.

## Resources

[Dan Abramov Redux Tutorials](https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867)
