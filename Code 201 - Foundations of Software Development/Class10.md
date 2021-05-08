# Error Handling & Debugging

## ORDER OF EXECUTION

To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

## EXECUTION CONTEXTS

The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope.
If you understand execution contexts (which have two stages) and stacks, you are more likely to find the error in your code.

## EXECUTION CONTEXT & HOISTING

Each time a script enters a new execution context, there are two phases of activity:

1. PREPARE

2. EXECUTE

If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code.
Error objects can help you find where your mistakes are and browsers have tools to help you read them.

## Types of Errors

JavaScript has 7 different types of errors. Each creates its own error object, which can tell you which line number and gives a description of the error.

1. Syntax Error (This is caused by incorrect use of the rules of the language)

2. Reference Error (This is caused by a variable that is not declared or is out of scope)

3. Eval Error (INCORRECT USE OF eval() FUNCTION )

4. URI Error (INCORRECT USE OF URI FUNCTIONS If these characters are not escaped in URls, they will cause an error: / ? & I : ; )

5. Type Error (This is often caused by trying to use an object or method that does not exist. )

6. Range Error (If you call a function using numbers outside of its accepted range. )

7. Error (The GENERIC ERROR OBJECT )

8. Nan (Actually its not an Error it's like datatype in the javascript but we will face it if we trying to do a mathimatical operation using two side one of them not a number )

**DEBUGGING is eliminating potential causes of an error.**

## BROWSER DEV TOOLS & JAVASCRIPT CONSOLE

The console is the developer friend we can use it to know where is , when and what the kind error we have

## HANDLING EXCEPTIONS

We can use try , catch and finally to handle any error that we don't expect it
