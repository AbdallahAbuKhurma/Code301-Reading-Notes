# How to write a script for a web page?

## HOW HTML, CSS, & JAVASCRIPT FIT TOGETHER:

* HTML: CONTENT LAYER. Html files this is where the content of the page lives. The HTML gives the page structure and adds semantics.

* {css} : PRESENTATION LAYER . css files The CSS enhances the HTML page with rules that state how the HTML content is presented (backgrounds, borders, box dimensions, colors, fonts, etc.).

* JavaScript (): BEHAVIOR LAYER .is files this is where we can change how the page behaves, adding interactivity. We will aim to keep as much of our JavaScript as possible in separate files.

## PROGRESSIVE ENHANCEMENT:

1. HTML ONLY Starting with the HTML layer allows you to focus on the most important thing about your site: it’s content. Being plain HTML, this layer should work on all kinds of devices, be accessible to all users, and load quite quickly on slow connections.

2. HTML+CSS Adding the CSS rules in a separate file keeps rules regarding how the page looks away from the content itself. You can use the same style sheet with all of your site, making your sites faster to load and easier to maintain. Or you can use different style sheets with the same content to create different views of the same data.

3. HTML+CSS+JAVASCRIPT the JavaScript is added last and enhances the usability of the page or the experience of interacting with the site. Keeping it separate means that the page still works if the user cannot load or run the JavaScript. You can also reuse the code on several pages (making the site faster to load and easier to maintain).

## How to use objects & methodes:
![](snip4.PNG)

* Basic JavaScript instructions:
A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.

### STATEMENTS ARE INSTRUCTIONS AND EACH ONE STARTS ON A NEW LINE:

 A statement is an individual instruction that the computer should follow. Each one should start on a new line and end with a semicolon. This makes your code easier to read and follow. The semicolon also tells the JavaScript interpreter when a step is over, indicating that it should move to the next step.

## COMMENTS:

You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code.

### There are two types of comments:

1. MULTI-LINE Comments: Multi-line comment s are often used for descriptions of how the script works, or to prevent a section of the script from running when testing it.  

2. SINGLE-LINE COMMENTS: Good use of comments will help you if you come back to your code after several days or months. They also help those who are new to your code.

## WHAT IS A VARIABLE?

A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.

• You may be able to do calculations like this in your head, but when writing a script to do this calculation, you need to give the computer very detailed instructions

## DATA TYPES:

1. NUMERIC DATA TYPE: The numeric data type handles numbers.

2. STRING DATA TYPE The strings data type consists of letters and other characters.

3. BOOLEAN DATA TYPE Boolean data types can have one of two values: true or false.

## RULES FOR NAMING VARIABLES:

1. The name must begin with a letter, dollar sign ($), or an underscore (_). It must not start with a number.

2. The name can contain letters, numbers, dollar sign ($), or an underscore (_). Note that you must not use a dash (-) or a period (.) in a variable name.

3. You cannot use keywords or reserved words. Keywords are special words that tell the interpreter to do something. For example, var is a keyword used to declare a variable. Reserved words are ones that may be used in a future version of JavaScript.

4. All variables are case sensitive, so score and Score would be different variable names, but it is bad practice to create two variables that have the same name using different cases.
