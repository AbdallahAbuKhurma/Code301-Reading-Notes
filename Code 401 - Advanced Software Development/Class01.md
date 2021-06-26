# Node Ecosystem, TDD, CI/CD

>

## What Array.map() does?

***The map()*** method in JavaScript creates an array by calling a specific function on each element present in the parent array. It is a non-mutating method. Generally map() method is used to iterate over an array and calling function on every element of array.

## What Array.reduce() does?

***The reduce()*** the function iterates over an array and runs a call back for each element. The callback receives the accumulator, the value and the index of the array element as parameters. The original array will never be harmed, The accumulator is a placeholder for what you want to return when the callback iteration is done running.

## Provide code snippets showing how to use superagent() to fetch data from a URL

### With normal Promise .then() syntax

    const getFecthedData = () => {

        const url = `www.example.com/API`;

        superagent.get(url).then(data => {
            
            const arrayOfData = data.body;
            
        }).catch(err => {
            console.log('==========');
            console.error(err);
            console.log('==========');
        });
    }

### With async / await syntax

    const getFecthedData = async () => {

        const url = `www.example.com/API`;

        awiat superagent.get(url).then(data => {
            
            const arrayOfData = data.body;
            
        }).catch(err => {
            console.log('==========');
            console.error(err);
            console.log('==========');
        });
    }

## Explain promises as though you were mentoring a Code 301 level student

A Promise is a proxy for a value not necessarily known when the promise is created. It allows you to associate handlers with an asynchronous action’s eventual success value or failure reason. This lets asynchronous methods return values like synchronous methods: instead of immediately returning the final value, the asynchronous method returns a promise to supply the value at some point in the future

## Are all callback functions considered to be Asynchronous? Why or Why Not?

The callback will be synchronous when the higher order function which calls it is calling it synchronously. Inversely if it is called within the context of the execution branch of an asynchronous operation it will be asynchronous.
