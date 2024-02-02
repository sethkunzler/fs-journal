# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > var, let, const

02. What is the definition of a function?

    > a function is an object block of code in javascript that takes an input and runs it through an operation to return an output.  

03. What are the `SOLID` principles?

    > I'll be honest, I don't remember seeing this anywhere in the reading and so I looked it up. it sounds like week 3 stuff to me though. we haven't even gone over classes in Javascript, and that's the first part of the SOLID which seems like applies strictly to js development logic -
    <br>* Single Responsibility Principle - where classes affect a single attribute
    <br>* Open-Closed Principle - open for extension but closed for modification
    <br>* Liskov Substitution Principle - in essence Refactoring Code for Rradability and simplicity
    <br>* Interface Segregation Principle - debugging based on device type, mac versus windows, modile vs desktop, chrome vs firefox, console or pc. that it works on all platforms.
    <br>* Dependency Inversion Principle - program to an interface and not an implementation


04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > 
    ```js
    // my answer 
    fruit[2] 
    // output: pineapple
    ```
05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }
    ```

    > 
    ``` js
    // my answer
    you.friends += them.name; // assigns Them to you's friends array
    them.friends += you.name; // assigns You to them's friends array
    ```

06. Give an example of a JavaScript `Conditional`:

    > 
    ```js
    jeremy {
        likesCats = true
    }
    // conditional example: 
    if (jermemy.likesCats == true) {
        console.log('this is the result of a conditional when true')
    } else {
        console.log('this is the result of a conditional when false')
    }
    // if the condition were based on numbers you could use cases as the conditional or add extra if statements before the last else statement 
    ```

07. What is the main difference between `parameters` and `arguments`?

    > parameters are set and arguments are supplied. arguments are typically supplied in the html file, or in other places the js file. the parameter is the conditon by which a function functions and is defined by the argument. 
    ```js 
    const arg1 = true;
    const arg2 = false;

    function twoParams(param1, param2) {
    // function statements
    }
    twoParams(arg1, arg2);
    ```

08. Instead of writing everything to the console, what is a better way to debug your code?

    > write with clarity. (prevention is the best protection) 
    "Always code as if the guy who ends up maintaining your code will be a violent psychopath who knows where you live." — John Woods
    <br> also adding in breakpoints or just utilizing that menu in your devtools

09. What is the difference between a `primitive` value and a `reference` value?

    > primitive value stores a single piece of information where a reference can store many of a specific set type. references are usually made of primitave values

10. Demonstrate a loop that prints the numbers between -100 and 100?

    
    ```js
    for(let i = -100; i <= 100; i++) {
        console.log(i) // log prints -100, -99, -98,.. 100 to the console 
    }
    ```
