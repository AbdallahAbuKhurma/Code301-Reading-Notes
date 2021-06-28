# Express REST API

>

## Review, Research, and Discussion

1. Name 3 real world use cases where you’d want to change the request with custom middleware

2. Login authentication

3. Logging data to get user insights

4. Error handling

5. True or false: The route handler is middleware?

    * False. A route handler can make requests and get responses without middleware. Middleware can be added to route handlers or other functions to alter/shape requests/responses.

6. In what ways can a middleware function end the process and send data to the browser?

    * Through the use of the next() Or 500 errors. If an error is triggered, it will end the WRRC and send the 500 message to the user through the broswer.

7. At what point in the request lifecycle can you “inject” middleware?

    * Middleware can be injected to shape the way the request object.

## Document the following Vocabulary Terms

* Middleware is software that lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications.

* Request Object is the main entry point for an application to issue a request to the Library - all operations on a URL must use a Request object. The request object is application independent in that both servers and clients use the same Request class.

* Response Object is the object which communicates between the server and the output which is sent to the client. To write an ASP page, all you need to do is write a standard HTML page, putting in the Active Server Pages script where needed.

* Application Middleware is middleware on a global level. this middleware executes on all route route calls.

* Routing Middleware is one of those middleware, what it does actualy is to take the original request, and forward it to a sub handler according to the path example : “/home” for a GET request is mapped to function getHome that handle it and eventually send a response to the client on the behalf of the original handler.

* Test Driven Development is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.

* Behavioral Testing is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    * Databases. Its interesting digging deeper on the fundamentals and seeing how everything is functioning.
    * REST and CRUD.
    * Request and Response Objects
    * Classes
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    * MongoDB
    * REST and CRUD terminology
    * Classes
3. What are you most excited about trying to implement or see how it works?
    * MONGO DB! Seems way more pratical than SQL.

## References

  [Using Express Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)

  [Review ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

  [Express Routing](https://expressjs.com/en/guide/routing.html)
