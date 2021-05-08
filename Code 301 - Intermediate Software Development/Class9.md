# What is functional programming?
>
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

## Pure functions

The first fundamental concept we learn when we want to understand functional programming is pure functions. But what does that really mean? What makes a function pure?

So how do we know if a function is pure or not? Here is a very strict definition of purity:

* It returns the same result if given the same arguments (it is also referred as deterministic)

* It does not cause any observable side effects

## Reading Files

If our function reads external files, it’s not a pure function — the file’s contents can change.

## Random number generation

Any function that relies on a random number generator cannot be pure.

## Pure functions benefits

The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:

* Given a parameter A → expect the function to return value B

* Given a parameter C → expect the function to return value D

A simple example would be a function to receive a collection of numbers and expect it to increment each element of this collection.

## Immutability

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

In Javascript we commonly use the for loop. This next for statement has some mutable variables.

## Referential transparency

Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

pure functions + immutable data = referential transparency.

## Functions as first-class entities

The idea of functions as first-class entities is that functions are also treated as values and used as data.
Functions as first-class entities can:

* refer to it from constants and variables

* pass it as a parameter to other functions

* return it as result from other functions

The idea is to treat functions as values and pass functions like data. This way we can combine different functions to create new functions with new behavior.

## Higher-order functions

When we talk about higher-order functions, we mean a function that either:

* takes one or more functions as arguments, or

* returns a function as its result

The doubleOperator function we implemented above is a higher-order function because it takes an operator function as an argument and uses it.

You’ve probably already heard about filter, map, and reduce. Let's take a look at these.

## Map

The idea of map is to transform a collection.

The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values.

## Reduce

The idea of reduce is to receive a function and a collection, and return a value created by combining the items.
