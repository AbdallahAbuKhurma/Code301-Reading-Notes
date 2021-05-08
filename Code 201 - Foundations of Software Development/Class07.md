# Object-Oriented Programming, HTML Tables

## Domain Modeling

Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

To define the same properties between many objects, you'll want to use a constructor function.

Here's an implementation of the EpicFailVideo constructor function.

var EpicFailVideo = function(epicRating, hasAnimals) {this.epicRating = epicRating; this.hasAnimals = hasAnimals; }

To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function.

## HTML 

### Tables

The table element is used to add tables to a web page.

A table is drawn out row by row. Each row is created with the tr element.

Inside each row there are a number of cells represented by the td element (or th if it is a header) .

You can make cells of a table span more than one row or column using the rowspan and colspan attributes.

For long tables you can split the table into a thead, tbody, and tfoot .

## JavaScript

### Functions, Methods, and Objects

Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).

***Example***

function updateMessage() {var el = document.getElementByld('message'}; el .textContent = msg;

sayHello();

if it has an information :

sayHello('Width','height');

* Functions allow you to group a set of related statements together that represent a single task.

* Functions can take parameters (information required to do their job) and may return a value.

* function('String',Number){any thing you want}

* An object is a series of variables and functions that represent something from the world around you.

***Example of object:***
let variables = {'first':10 , 'second':20}

In an object, variables are known as properties of the object; functions are known as methods of the object.

Web browsers implement objects that represent both the browser window and the document loaded into the browser window.

### JavaScript also has several built-in objects such as :

1. String

2. Number

3. Math

4. Date

Arrays and objects can be used to create complex data sets .
