# Passing Functions as Props

## Lifting State Up

"Often, several components need to reflect the same changing data. We recommend lifting the shared state up to their closest common ancestor. Let’s see how this works in action.

In this section, we will create a temperature calculator that calculates whether the water would boil at a given temperature.

Next, we will create a component called Calculator. It renders an (input) that lets you enter the temperature, and keeps its value in this.state.temperature.

### Adding a Second Input

Our new requirement is that, in addition to a Celsius input, we provide a Fahrenheit input, and they are kept in sync.

We can start by extracting a TemperatureInput component from Calculator. We will add a new scale prop to it that can either be "c" or "f":

We have two inputs now, but when you enter the temperature in one of them, the other doesn’t update. This contradicts our requirement: we want to keep them in sync.

We also can’t display the BoilingVerdict from Calculator. The Calculator doesn’t know the current temperature because it is hidden inside the TemperatureInput

### Writing Conversion Functions

First, we will write two functions to convert from Celsius to Fahrenheit and back:

These two functions convert numbers. We will write another function that takes a string temperature and a converter function as arguments and returns a string. We will use it to calculate the value of one input based on the other input.

It returns an empty string on an invalid temperature, and it keeps the output rounded to the third decimal place:

Lifting State Up
Currently, both TemperatureInput components independently keep their values in the local state:

However, we want these two inputs to be in sync with each other. When we update the Celsius input, the Fahrenheit input should reflect the converted temperature, and vice versa.

In React, sharing state is accomplished by moving it up to the closest common ancestor of the components that need it. This is called “lifting state up”. We will remove the local state from the TemperatureInput and move it into the Calculator instead.

If the Calculator owns the shared state, it becomes the “source of truth” for the current temperature in both inputs. It can instruct them both to have values that are consistent with each other. Since the props of both TemperatureInput components are coming from the same parent Calculator component, the two inputs will always be in sync.

Let’s see how this works step by step.

First, we will replace this.state.temperature with this.props.temperature in the TemperatureInput component. For now, let’s pretend this.props.temperature already exists, although we will need to pass it from the Calculator in the future:"

### Recap

* React calls the function specified as onChange on the DOM (input). In our case, this is the handleChange method in the TemperatureInput component.

* The handleChange method in the TemperatureInput component calls this.props.onTemperatureChange() with the new desired value. Its props, including onTemperatureChange, were provided by its parent component, the Calculator.

* When it previously rendered, the Calculator had specified that onTemperatureChange of the Celsius TemperatureInput is the Calculator’s handleCelsiusChange method, and onTemperatureChange of the Fahrenheit TemperatureInput is the Calculator’s handleFahrenheitChange method. So either of these two Calculator methods gets called depending on which input we edited.

* Inside these methods, the Calculator component asks React to re-render itself by calling this.setState() with the new input value and the current scale of the input we just edited.

* React calls the Calculator component’s render method to learn what the UI should look like. The values of both inputs are recomputed based on the current temperature and the active scale. The temperature conversion is performed here.

* React calls the render methods of the individual TemperatureInput components with their new props specified by the Calculator. It learns what their UI should look like.

* React calls the render method of the BoilingVerdict component, passing the temperature in Celsius as its props.

* React DOM updates the DOM with the boiling verdict and to match the desired input values. The input we just edited receives its current value, and the other input is updated to the temperature after conversion.

* Every update goes through the same steps so the inputs stay in sync.

## Lists and Keys

First, let’s review how you transform lists in JavaScript.

Given the code below, we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:

"### Rendering Multiple Components

You can build collections of elements and include them in JSX using curly braces {}.

Below, we loop through the numbers array using the JavaScript map() function. We return a (li) element for each item. Finally, we assign the resulting array of elements to listItems

### Basic List Component

Usually you would render lists inside a component.

We can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.

When you run this code, you’ll be given a warning that a key should be provided for list items. A “key” is a special string attribute you need to include when creating lists of elements. We’ll discuss why it’s important in the next section.

Let’s assign a key to our list items inside numbers.map() and fix the missing key issue.

### Keys

Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

The best way to pick a key is to use a string that uniquely identifies a list item among its siblings. Most often you would use IDs from your data as keys:

When you don’t have stable IDs for rendered items, you may use the item index as a key as a last resort:

### Extracting Components with Keys

Keys only make sense in the context of the surrounding array."

For example, if you extract a ListItem component, you should keep the key on the (ListItem ) elements in the array rather than on the (li) element in the ListItem itself.

## How to Use the Spread Operator (…) in JavaScript

"The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

### What is the spread operator?

InJavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

“When ...arr is used in the function call, it ‘expands’ an iterable object arr into the list of arguments.” — JavaScript.info

The spread operator was added to JavaScript in ES6 (ES2015), just like the rest parameters, which have the same syntax: three magic dots …

### What is ... used for?

“Spread operator to the rescue! It looks similar to rest parameters, also using ..., but does quite the opposite.” — JavaScript.info

### What else can … do?

The … spread operator is useful for many different routine tasks in JavaScript, including the following:

* Copying an array

* Concatenating or combining arrays

* Using Math functions

* Using an array as arguments

* Adding an item to a list

* Adding to state in React

* Combining objects

* Converting NodeList to an array

* In each case, the spread syntax expands an iterable object, usually an array, though it can be used on any interable, including a string.

### Copying an array

Using the … spread operator is a convenient way to copy an array or combine arrays, and it can even add new items:

### Adding to state in React

Adding an item to an array in React state is easily accomplished using the spread operator. Take the following example adapted from my article on how to add to an array in React State:

### Combining objects

The spread syntax is useful for combining the properties and methods on objects into a new object:

### Conclusion

“The spread operator can expand another item by split an iterable element like a string or an array into individual elements:” — CodinGame.com"

[Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)

[Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)

[How to Use the Spread Operator (…) in JavaScript](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
